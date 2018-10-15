# Code intelligence overview

Code intelligence provides advanced code navigation and cross-references for your code on Sourcegraph, your code host, and your code review tools:

- Hover tooltips with documentation and type signatures
- Go-to-definition
- Find references
- Symbol search

Code intelligence is provided by language servers that run securely in your self-hosted Sourcegraph instance. These language servers perform advanced, scalable code analysis and are derived from our popular open-source language servers in use by hundreds of thousands of developers in editors and on Sourcegraph.com.

By spinning up Sourcegraph, you can get code intelligence:

- On the Sourcegraph web interface
- On code files on your code host, via our [integrations](/integration.md)
- On diffs in your code review tool, via our [integrations](/integration.md)
- Via the Sourcegraph API (for programmatic access)

<div class="code-intel-images">

<div>

**Hover tooltips with documentation and type signatures**

<img src="img/hover-tooltip.png" width="500"/>

</div>

<div>

**Go to definition**

<img src="img/go-to-def.gif" width="500"/>

</div>

<div>

**Find references**

<img src="img/find-refs.gif" width="450"/>

</div>

<div>

**GitHub pull request and file integration**

<img src="img/CodeReview.gif" width="450" style="margin-left:0;margin-right:0;"/>

</div>

<div>

**Symbol search**

<img src="img/Symbols.png" width="500"/>

</div>

<div>

**Symbol sidebar**

<img src="img/SymbolSidebar.png" width="500"/>

</div>

</div>

<div style="clear:both">&nbsp;</div>

---

## Languages

Sourcegraph's code intelligence supports code written in the following programming languages:

- [Go](/extensions/language_servers/go.md)
- [JavaScript](/extensions/language_servers/javascript.md)
- [TypeScript](/extensions/language_servers/typescript.md)
- [Python](/extensions/language_servers/python.md)
- [Java](/extensions/language_servers/java.md)
- [PHP](/extensions/language_servers/php.md)
- [Bash](/extensions/language_servers/experimental_language_servers.md)
- [Clojure](/extensions/language_servers/experimental_language_servers.md)
- [C++](/extensions/language_servers/experimental_language_servers.md)
- [C#](/extensions/language_servers/experimental_language_servers.md)
- [CSS](/extensions/language_servers/experimental_language_servers.md)
- [Dockerfile](/extensions/language_servers/experimental_language_servers.md)
- [Elixir](/extensions/language_servers/experimental_language_servers.md)
- [HTML](/extensions/language_servers/experimental_language_servers.md)
- [Lua](/extensions/language_servers/experimental_language_servers.md)
- [OCaml](/extensions/language_servers/experimental_language_servers.md)
- [R](/extensions/language_servers/experimental_language_servers.md)
- [Ruby](/extensions/language_servers/experimental_language_servers.md)
- [Rust](/extensions/language_servers/experimental_language_servers.md)
- [Swift](/extensions/language_servers/swift.md)

Interested in a language that's not listed here? Post or subscribe to an issue for the language on the [Sourcegraph issue tracker](https://github.com/sourcegraph/issues/issues). [Contact us](https://about.sourcegraph.com/contact) if your organization would like to expedite development of a particular language.

### Open standards

Code intelligence is powered by language servers based on the open-standard Language Server Protocol (published by Microsoft, with participation from Facebook, Google, Sourcegraph, GitHub, RedHat, Twitter, Salesforce, Eclipse, and others).

Hundreds of thousands of developers already use Sourcegraph's language servers in their editor or while browsing public code on [Sourcegraph.com](https://sourcegraph.com). Microsoft's [Visual Studio Code](https://code.visualstudio.com) and GitHub's [Atom](https://atom.io) editors both use Sourcegraph language servers in official editor extensions. The language servers used for code intelligence on Sourcegraph are based on our widely used language servers, with extensive improvements for performance, cross-repository definitions and references, security, isolation, type/build inference, and robustness.

For more information about the Language Server Protocol (LSP), visit [Microsoft's official LSP site](https://microsoft.github.io/language-server-protocol/). For a more detailed list of existing language servers, visit [langserver.org](https://langserver.org) (maintained by Sourcegraph).

If you're a language server developer, see [documentation on adapting a language server to work with Sourcegraph](/extensions/language_servers/adapting_existing_language_servers.md).

---

## Getting started

- [Set up code intelligence on Sourcegraph (for single-node `sourcegraph/server` deployments)](/extensions/language_servers/install/index.md)
- [Set up code intelligence on Sourcegraph (for Kubernetes cluster deployments)](https://github.com/sourcegraph/deploy-sourcegraph/blob/master/docs/install.md#add-language-servers-for-code-intelligence)

Interested in trying it out on public code? See [this sample file](https://sourcegraph.com/github.com/dgrijalva/jwt-go/-/blob/token.go#L37:6$references) on Sourcegraph.com.
