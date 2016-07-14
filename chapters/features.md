# Features

_In this chapter, I will review the current features we use and why we use them._

##### SSL Offloading

SSL Offloading is the term used to terminate SSL/TLS (HTTPS traffic) before the traffic reaches its destination, this reduces the processing burden of encrypting and decrypting traffic on the application server.

We currently use SSL offloading on our marketing websites, uploads portal and customer portal. The plan in the next year is to increase the number of services accepting HTTPS traffic, so we need to make sure our end solution can scale SSL offloading to meet our needs in the future.

##### 