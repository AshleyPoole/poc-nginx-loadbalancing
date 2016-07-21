# Loadbalancer.org Pros vs. Cons


### Pros

- Due to the cost and the concomitant to Loadbalancer.org, we're able to get a good discount for internal load balancers.
- The appliances are fully supported.
- Loadbalancer.org has a GUI for users to modify
- Loadbalancer.org provides both Layer 7 and Layer 4 load balancing solutions; this could be beneficial for future projects.
- Loadbalancer.org has a WAF feature that allows requests to be scanned for hacking attempts.
- Loadbalancer.org provides the ability to add manual parameters to the HA Proxy configuration.

### Cons

- When contacting loadbalancer.org for support, you get redirected to a call centre service. Calls are then responded to in a first come, first, serve fashion vs. urgency. A recent example took 10 minutes for a recall but took 3 hours to return a fix, in this time I was able to resolve the issue entirely myself even with limited knowledge of how the system works.
- In the past few months, we've had many problems with their recent upgrade; this has affected production websites.
- To scale loadbalancer.org appliances you have to scale vertically (adding more RAM/CPU).
- When adding manual parameters to the HA Proxy configuration, it locks the GUI.
- There are many steps involved in adding a new VIP to the loadbalancer.org appliance, and this can't be automated.
- Loadbalancer.org currently does not support Lets Encrypt and has said they will never to support it.
- Loadbalancer.org currently do not support [HTTP/2](https://www.cloudflare.com/http2/), and application discovery. 
