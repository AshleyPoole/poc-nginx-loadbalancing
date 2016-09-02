# F5 Pros vs. Cons


### Pros

- F5 have an established product, and include every feature that we require.
- F5 already have a WAF module with an extensive feature set, although this is a licenced extra. 
- F5 offer both physical and virtual appliances, with the physical appliance we could use partitioning to have DMZ and internal traffic on one device.

### Cons

- Although not an initial requirement, F5 does't have an auto scale feature like AVI. It also does't have the analytics.
- F5 don't offer true Active/Active; With F5 you split the VIPs across load balancers, so _x_ number of VIPs are active on each load balancer.
- F5's licencing works on how much traffic is processed, this means when we grow we'll need to renegotiate licencing. Additionally, if we purchase physical devices, we may need a hardware refresh.
- Gartner reported the following in its [latest report](https://www.gartner.com/doc/reprints?id=1-3GEK4YV&ct=160830&st=sb&mkt_tok=eyJpIjoiT0RNeE5tTXpPREJrWTJabCIsInQiOiI0OUZoQkVwYjhvcFwvc0FueWh3MnRQZU90RWZ3a0lESzFneHVaaitjRzZNYytIWWFFYWFVTkN4TTNXbEU5b2hUZ1oyZTdLTTlDV1hsYWFySFpxMUZrNFFSQ1Q1MnFGcnVNN28rWnlaZ293ZHM9In0%3D) on ADC's "Based on client feedback and deals that Gartner reviews, F5 is the most expensive ADC vendor in the market."
- Gartner also said the following "The F5 platform is not well-aligned with midmarket and SMB organizations' ADC requirements from feature and price perspectives."
