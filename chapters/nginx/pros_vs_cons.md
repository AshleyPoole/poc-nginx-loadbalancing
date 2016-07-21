# NGINX Pros vs. Cons


### Pros

- To improve management and reduce the risk of issues we could use [Chef](https://chef.io/) to fully manage the installation and configuration of the load balancer nodes. We can leverage our existing in-house Chef knowledge.
- Due to the low cost of each node, we could have dedicated nodes for Internal/External traffic, as well as dedicated nodes for each environment (DEV, QA, PROD).
- Due to fully building the system, we'll be able to document each configuration file, as well as know where to look if a problem arises.
- Using a service like Lets Encrypt will dramatically reduce the cost of purchasing SSL certificates, as well as allow new projects to accept HTTPS traffic by default. Let's Encrypt will also reduce technical debt as certificates are automatically renewed each month, and last for three months.
- Using NGINX along with BGP, we're able to progress towards using active/active technologies. As we scale, we'll also be able to increase the number of load balancer nodes vs. increasing the specs as traffic will be evenly distributed between load balancer nodes.
- With the purchase of [NGINX Plus](https://www.nginx.com/products/pricing/) we can get support for any NGINX issue.
- Loadbalancer nodes are not physical so are not subject to hardware issues or scaling issues if we need better hardware. This also prevents us with being left with a brick if/when we move service into the cloud.
- NGINX supports [HTTP/2](https://www.cloudflare.com/http2/) out of the box, this would allow fast loading of our websites.


### Cons

- Any load balancer issues not related to NGINX would have to be resolved by ourselves. This risk would be offset by using configuration management ([Chef](https://www.chef.io/)), stable versions of software, documenting every change on the box, and the reason for the change. All changes will be made in source control using Stash.
- No GUI; NGINX Plus comes with a GUI to monitor the status of the load balancer node. However, it does not allow any changes to the configuration. NGINX Plus does, however, have an API that allows configuration. If picked for the load balancing solution I would create two tools for managing the load balancer nodes.
  - A PowerShell module used to drain/offline services/nodes.
  - A program to configure NGINX with a YAML file that can be stored in Stash for developer changes (like our current configuration repo)
