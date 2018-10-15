# Site configuration

Sourcegraph is configured by a site configuration JSON file. To view and edit your site configuration on the web-based site admin, go to the configuration page by clicking **Admin** in the top right of any page, and going to **Configuration** in the left side menu. (The URL is `https://sourcegraph.example.com/site-admin/configuration`.)

For Kubernetes cluster deployments of Sourcegraph, edit the `config-file.ConfigMap.yaml` file and then use `kubectl apply -f ...` to update the resource.

<div style="padding-bottom:67.1%;height:0;position:relative;overflow:hidden">
    <img src="img/Admin.png" width="800" class="flex br2 ba pa2 b--light-8 mv4 center"/>
</div>

---

## Next steps

See [all site configuration options](/admin/site_config), or read walkthroughs of common configuration use cases:

- [Add repositories to search from your code host](/admin/repo/add)
- [Add user authentication providers (SSO)](/admin/auth)
- [Configure search scopes](/user/search/scopes)
- [Integrate with Phabricator](/integration/phabricator)
- [Add organizations](/user/organizations)
- [Add a TLS/SSL certificate](/admin/tls_ssl)
- [Use a custom domain](/admin/url)
- [Updating Sourcegraph Server](/admin/updates)
