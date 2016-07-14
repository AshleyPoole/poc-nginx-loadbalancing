# NGINX Pros vs. Cons


### Pros

- To improve management and reduce risk of issues we could use [Chef](https://chef.io/) to fully manage the installation and configuration of the loadbalancer nodes.
- Due to the low cost of each node, we could have dedicated nodes for Internal/External traffic, as well as dedicated nodes for each environment (DEV,QA,PROD).
- Due to fully building the system, we'll be able to document each configuration file, as well as know where to look if a problem arises.
- Using a service like Lets Encrypt will dramatically reduce the cost of purchasing SSL certificates, as well as allow new projects to accept HTTPS traffic by default. Lets Encrypt will also reduce technical debt as certificates are automatically renewed each month, and last for 3 months.
- Using NGINX along with BGP, were able to progress with our project of using active/active technologies. As we scale we'll also be able to increase the number of load balancer nodes vs increasing the specs as traffic will be evenly distributed between load balancer nodes.
- With the purchase of [NGINX Plus](https://www.nginx.com/products/pricing/) we can get support for any NGINX issue.
- Loadbalancer nodes are not physical so are not subject to hardware issues or scaling issues if we need better hardware. 


### Cons

- Any loadbalancer issues not related to NGINX would have to be resolved by ourselves. This risk would be offset by using configuration management ([Chef](https://www.chef.io/)) as well as documentation every change on the box as well as reason for the change. Changes will also be made using Chef with Stash.
- No GUI, NGINX Plus comes with a GUI to monitor the status of the loadbalancer node, however does not allow any changes to the configuration. NGINX Plus does however have an API that allow configuration. If successfully picked for the load balancing solution I would create two tools for managing the loadbalancer nodes.
  - A PowerShell module used to drain/offline services/nodes.
  - A program to configure NGINX with a YAML file that can be stored in Stash for developer changes (Like our current configuration repo)