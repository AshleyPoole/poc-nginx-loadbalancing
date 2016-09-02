# Loadbalancer.org Pros vs. Cons


### Pros

- Due to the cost and the commitment to Loadbalancer.org, we're able to get a discount for internal load balancers. We're also able to get free load balancers for our Dev/QA environments.
- Loadbalancer.org has a web interface for users to modify and configure our VIPs.
- Loadbalancer.org has a built in WAF feature; If configured correctly this could allow us to move away from the Dell WAF.
- Loadbalancer.org has an HA Proxy backend, and it's possible to add additional parameters that may not be found in the GUI.

### Cons

- When contacting loadbalancer.org for support, you get redirected to a call centre service. Calls are then responded to in a "first come, first, served" fashion vs. urgency. A recent example took 10 minutes for a callback but took 3 hours to return a fix, in this time I was able to resolve the issue entirely myself even with limited knowledge of how the system works.
- In the past few months, we've had many problems with their recent upgrade; This has affected production websites.
- loadbalancer.org are unable to demonstrate an active/active configuration of any type, due to this if we wished to scale, we'd have to scale vertically, this, however, can be done without any additional licences, unlike competitors. 
- When adding manual parameters to the HA Proxy configuration, it locks the GUI; This can be an problem as it limits what changes we can make.
- There are many steps involved in adding a new VIP to the loadbalancer.org appliance, and this can't be automated.
- Loadbalancer.org currently does not support Let's Encrypt and has said they will never to support it. This, unfortunately, means we'd have to create something (un-supported) custom to benefit from Let's Encrypt.
