# Load-balancing using NGINX

In this document, I will highlight the pros and cons of using NGINX Plus for our load-balancing solution. For the following document, I will assume the following requirements:

- The end solution will be deployed at each business location.
- The end solution should be scalable and be able to handle a minimum of 100Mb/s
- The end solution should have examples of handling 1Gb/s for future scalability options.
- The end solution should be easily managed as part of the goal for continuous delivery.
- The end solution should match the same feature set of our current load balancers.
  - Allow easy configuration via an API/CLI module.
  - Support `X-Forwarded-For` header injection.
  - Support termination of HTTPS traffic.
  - Support weighted node values.
  - Support session persistence.
  - Support custom heath checks to be defined.
  - Support a custom 'Gone Fishing' page if node health checks fail.
  - Support high availability via active/active or active/passive
