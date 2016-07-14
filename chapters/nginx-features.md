# NGINX Features

In this chapter I will list the features supported with a NGINX loadbalancer, including features included in NGINX Plus.

NGINX supports the following features from our current feature list:

- SSL Offloading
- Session Persistence*
- Health Checks
- Fallback Server (Gone Fishin')
- API/CLI Commands*
- Weighted nodes


A custom build solution using NGINX could also include the following features:

##### Lets Encrypt

Lets Encrypt is a free and open source tool/provider for getting SSL certifcates. They provide a CLI tool that allows anyone to verify their domain and create certs. Lets Encrypt currently only support Linux distributions.

The benefit of Lets Encrypt is the ability to create as many certificates as we want for free with no comparison in the type of security we get from our current certificates.

##### Scale (Active/Active)

Most load balancing technologies dont support active/active solutions, however combined with BGP we could have both loadbalancers accept and manage requests.

This is done by the loadbalancers advertising the IPs it owns to the router. The router then will round-robin requests to each loadbalancer, which will then reverse proxy requests to the application nodes.

This solution has been replicated in many organisations allowing for higher scalability and better prevention to DDoS attacks.

##### Service Discovery*

Service Discovery is the ability to contact an application without knowing what host it lives on. This is generally done using DNS along with [Consul](https://www.consul.io/).

An application would be able to ask for `Payment-API.service.consul` and have that resolve to application node. This happens as when the service starts up it registers it's self with a health API. This allows only health nodes to be descovered.

----

```
* = Only avalable in NGINX Plus.
```