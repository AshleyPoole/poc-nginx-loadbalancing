# Load-balancing using NGINX

In this document, I will highlight the pros and cons of using NGINX for our load-balancing solution. For the following document, I will assume the following requirements:

- The end solution will be deployed at each business location.
- The end solution should be scalable and be able to handle a minimum of 100Mb/s and should have examples of going well beyond 1Gb/s for future scalability options.
- The end solution should be easily managed as part of the goal for continuous delivery.
- The end solution should match the same feature set of our current load balancers.
  - Allow easy configuration via an API/CLI module.
  - Allow `X-Forwarded-For` header to be injected.
  - Allow termination of HTTPS traffic.
  - Allow weighted node values.
  - Allow session persistence.
  - Allow custom heath checks to be defined.
  - Allow a 'Gone Fishing' page if node health checks fail.