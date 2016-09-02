# F5 Pros vs. Cons


### Pros

- F5 are the market leaders, due to this all features that we require already exist.
- F5 already have a WAF module with an extensive feature set, although this is a licenced extra. 
- F5 offer both physical and virtual appliances, with the physical appliance we could use partitioning to have DMZ and internal traffic on one device.

### Cons

- Although not an initial requirement, F5 does't have an auto scale feature like AVI. It also does't have the analytics.
- F5 don't offer true Active/Active; With F5 you split the VIPs across load balancers, so _x_ number of VIPs are active on each load balancer.
- F5's licencing works on how much traffic is processed, this means when we scale we'll need to renegotiate licencing. Additionally, if we purchase physical devices, we may need a hardware refresh.