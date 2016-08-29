# Features

In this chapter, I will list the main selling points of Avi Networks
distributed load balancer.

The Avi load balancer has six core categories, each with features that set them
apart from other load balancer solutions.

##### Application Availability
In this category we tick off most of the requirements for our load balancer
solution; health monitoring, session persistence, stand-in error page, weighted
load balancing and high availability. Where Avi shines in this category is the
ability to scale horizontally and autoscale. (This uses an integration with
vSphere to automatically scale -- Without human intervention, this can be
programmed to scale with our traffic or when a load balancer engine fails, this
process can be done in less than 30 seconds).

##### Application Security
Our only requirement from this category was SSL offloading, but Avi has a lot
of extra features we would benefit from, a few examples include the ability to
detect and prevent L3/L4/L7 DDoS attacks and block IPs within the management
interface. Another advantage Avi has is rate limiting; this would limit the
number of requests made by security scanners. In Q1 of 2017 Avi will also have
a built in WAF, this in combination with the ability to block IPs directly from
the load balancer will make it much easier to mitigate attacks.

##### App Performance Monitoring
Another category where Avi shines is Monitoring/Analytics. After logging into
Avi and selecting a VIP/service, you're presented with a table of page requests
and page load time metrics; this can be filtered by a multitude of things like
country, IP, browser, device type, etc. (See screenshot).  These tools can be
used for marketing purposes to make sure customers can load our site in an
acceptable time; we can also identify what errors customers are getting and
even what scan attacks are taking place.

##### Application Optimisation
This category is short, Avi like many other load balancing solutions provide
content caching so resources like images, JavaScript and CSS are served from
local cache vs. spending time on a round trip to the backend servers. Avi also
has the ability to resize images on the fly.

##### Programmability
Avi has a few methods for automating configuration via their core REST API:
Chef, Puppet, SaltStack, and a CLI tool. *** I'm currently researching to see
if a PowerShell Module exists ***

##### Management
One thing we want to focus on when selecting our load balancing solution is
ease of management and reducing the amount of human intervention needed.  Avi
has many features we could benefit from, I've already touched on the REST API,
so I'll mention the GUI functions: one of the main ones being multi-tenant
mode. In theory, this would allow a management node in each location in HA mode
and allow configuration of the UK from the US node.  Another feature Avi has is
templates: when adding a VIP/Service you can select from a number of pre-made
or custom templates to make the whole setup that much easier.
