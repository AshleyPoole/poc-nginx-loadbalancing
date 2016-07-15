# Loadbalancer.org


#### Going to DEV instance.

```
$ > httpd-2.4.23-x64-vc14\Apache24\bin\ab.exe -n 50000 -c 200 http://devuk.www.protolabs.co.uk/
This is ApacheBench, Version 2.3 <$Revision: 1748469 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking devuk.www.protolabs.co.uk (be patient)
Completed 5000 requests
Completed 10000 requests
Completed 15000 requests
Completed 20000 requests
Completed 25000 requests
Completed 30000 requests
Completed 35000 requests
Completed 40000 requests
Completed 45000 requests
Completed 50000 requests
Finished 50000 requests


Server Software:        Microsoft-IIS/7.5
Server Hostname:        devuk.www.protolabs.co.uk
Server Port:            80

Document Path:          /
Document Length:        33752 bytes

Concurrency Level:      200
Time taken for tests:   785.821 seconds
Complete requests:      50000
Failed requests:        476
   (Connect: 0, Receive: 0, Length: 476, Exceptions: 0)
Non-2xx responses:      476
Total transferred:      1691728156 bytes
HTML transferred:       1671584110 bytes
Requests per second:    63.63 [#/sec] (mean)
Time per request:       3143.285 [ms] (mean)
Time per request:       15.716 [ms] (mean, across all concurrent requests)
Transfer rate:          2102.36 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    2   2.5      1     100
Processing:   245 3040 5816.7   2051   75482
Waiting:       35 3035 5817.0   2046   75479
Total:        247 3042 5816.7   2053   75483

Percentage of the requests served within a certain time (ms)
  50%   2053
  66%   2133
  75%   2218
  80%   2326
  90%   2993
  95%   4955
  98%  15107
  99%  33153
 100%  75483 (longest request)
 ```
 
 #### Going to PROD instance
 
 
 ```
 b -n 50000 -c 200 http://www.protolabs.co.uk/
This is ApacheBench, Version 2.3 <$Revision: 1706008 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking www.protolabs.co.uk (be patient)
Completed 5000 requests
Completed 10000 requests
Completed 15000 requests
Completed 20000 requests
Completed 25000 requests
Completed 30000 requests
Completed 35000 requests
Completed 40000 requests
Completed 45000 requests
Completed 50000 requests
Finished 50000 requests


Server Software:
Server Hostname:        www.protolabs.co.uk
Server Port:            80

Document Path:          /
Document Length:        26321 bytes

Concurrency Level:      200
Time taken for tests:   417.524 seconds
Complete requests:      50000
Failed requests:        0
Total transferred:      1336560000 bytes
HTML transferred:       1316050000 bytes
Requests per second:    119.75 [#/sec] (mean)
Time per request:       1670.096 [ms] (mean)
Time per request:       8.350 [ms] (mean, across all concurrent requests)
Transfer rate:          3126.13 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        8   10   4.9      9    1005
Processing:    58 1657 306.4   1602    3411
Waiting:       46 1645 307.0   1591    3401
Total:         67 1667 306.0   1612    3420

Percentage of the requests served within a certain time (ms)
  50%   1612
  66%   1663
  75%   1710
  80%   1750
  90%   1911
  95%   2340
  98%   2653
  99%   2808
 100%   3420 (longest request)
 ```