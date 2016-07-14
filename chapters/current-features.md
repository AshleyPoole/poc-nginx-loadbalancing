# Current Features

In this chapter, I will review the current features we have, what why are and why we use them.

##### SSL Offloading

SSL Offloading is the term used to terminate SSL/TLS (HTTPS traffic) before the traffic reaches its destination, this reduces the processing burden of encrypting and decrypting traffic on the application server.

We currently use SSL offloading on our marketing websites, uploads portal and customer portal. The plan in the next year is to increase the number of services accepting HTTPS traffic, so we need to make sure our end solution can scale SSL offloading to meet our needs in the future.

##### Session Persistence

Session Persistence is the team used to direct an end-user continuously to a particular node until the end of their session. This can be useful if the application uses sessions to temporarily save user data.

Session Persistence is currently setup on two of our applications, we have projects to remove this requirement however this is a long term project.

##### High Availability

This feature is one of the core features of any loadbalancer, most implementations use a heartbeat between both loadbalancer nodes and activate  floating IPs if connection is lost between them.

##### Health Checks

Health checks give us a way to periodically poll end nodes to find out if the application is performing as expected. 

At the moment we only check if the site returns the HTTP code of 200 (OK) however there are plans on doing more rigorous tests to ensure users are having the best experience with our sites and not experiencing issues.

##### Fallback Server (Gone Fishin')

The Fallback Server feature provides us the ability to show end-users a marketing approved message that says were in planned maintenance, this can be useful when were doing planned maintenance (Updates or DR tests) as well as when nodes fail health checks.

##### API/CLI Commands

To allow future integrations with deployment pipelines we require a way to interface with the loadbalacing solution without human intervention, this comes in the from of a REST API or CLI commands that can be scripted. 

Currently we manually change the status of our nodes via the GUI however a PowerShell module was created. The plan would be to use this module with the next iteration of the deployment system.

##### Weighted nodes

Currently we don't use weighted nodes as we round-robin requested to our application nodes, however future projects may rely on this feature to change the distribution of traffic.

An example use case would be the ability to canary deployments allowing faster iteration and reduction in issues.