# F5 Pros vs. Cons


### Pros

- F5 are the market leaders, due to this all features that we require already exist with their solution.
- F5 already have a WAF module with an extensive feature set, although this is a licenced extra. 
- F5 offer both physical and virtual appliances, with the physical appliance we could use partitioning to have DMZ and internal traffic on one device.

### Cons

- Although not an initial requirement, F5 does not have an auto scale feature like AVI. It also does not have the analytics.
- F5 don't offer true Active/Active; with F5 you have to split the VIPs so _x_ number of VIPs are active on each load balancer.