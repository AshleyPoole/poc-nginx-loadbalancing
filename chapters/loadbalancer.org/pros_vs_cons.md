# Loadbalancer.org Pros vs. Cons


### Pros

- Due to the cost and the concomitant to Loadbalancer.org we're able to get a good discount for internal loadbalancers.
- The appliances are fully supported.
- Loadbalancer.org has a GUI for users to modify 
- Loadbalancer.org provides both Layer 7 and Layer 4 loadbalancing solutions, this could be beneficial for future projects.
- Loadbalancer.org has a WAF feature that allows requests to be scanned for hacking attempts.
- Loadbalancer.org provides the ability to add manual parameters to the HA Proxy configuration.
- Loadbalancer.org provides 

### Cons

- When contacting loadbalancer.org for support you get redirected to a call center service. Calls are then responded to in a first come, first serve fashion vs urgency. A resent example took 10 minutes for a re-call but took 3 hours to return a fix, in this time I was able to fully fix the issue myself even with limited knowledge of how the system works.
- In the past few months we've had many issues with there resent upgrade, this has affected production websites.
- To scale loadbalancer.org appliances you have to scale vertical (adding more  RAM/CPU).
- When adding manual perimeters to the HA Proxy configuration, it locks the GUI. 
- There are many steps of adding a new VIP to the loadbalancer.org appliance, and this cant be automated.
- Loadbalancer.org currently does not support Lets Encrypt, and has said to never support it.
