# NGINX Pros vs. Cons


### Pros

- To improve management and reduce risk of issues we could use [Chef](https://chef.io/) to fully manage the installation and configuration of the loadbalancer nodes.
- Due to the low cost of each node, we could have dedicated nodes for Internal/External traffic, as well as dedicated nodes for each environment (DEV,QA,PROD).
- Due to fully building the system, we'll be able to document each configuration file, as well as know where to look if a problem arises.
- Using a service like Lets Encrypt will dramatically reduce the cost of purchasing SSL certificates, as well as allow new projects to accept HTTPS traffic by default. Lets Encrypt will also reduce technical debt as certificates are automatically renewed each month, and last for 3 months.
- Using NGINX along with BGP, were able to progress with our project of using active/active technologies. As we scale we'll also be able to increase the number of load balancer nodes vs increasing the specs as traffic will be evenly distributed between load balancer nodes.
- With the purchase of [NGINX Plus](https://www.nginx.com/products/pricing/) we can get support for any NGINX issue.
- Loadbalancer nodes and easily be moved as they would be virtual.


### Cons

- 