# NGINX

#### Going to DEV instance.

```
$ > httpd-2.4.23-x64-vc14\Apache24\bin\ab.exe -n 50000 -c 200 http://devuk.www.*.co.uk/
This is ApacheBench, Version 2.3 <$Revision: 1748469 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking devuk.www.*.co.uk (be patient)
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


Server Software:        nginx/1.9.13
Server Hostname:        devuk.www.*.co.uk
Server Port:            80

Document Path:          /
Document Length:        33752 bytes

Concurrency Level:      200
Time taken for tests:   800.768 seconds
Complete requests:      50000
Failed requests:        0
Total transferred:      1707050000 bytes
HTML transferred:       1687600000 bytes
Requests per second:    62.44 [#/sec] (mean)
Time per request:       3203.071 [ms] (mean)
Time per request:       16.015 [ms] (mean, across all concurrent requests)
Transfer rate:          2081.80 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    2   6.4      1    1003
Processing:   256 3195 386.5   3100    8339
Waiting:      245 3191 385.8   3096    8337
Total:        257 3196 386.4   3101    8340

Percentage of the requests served within a certain time (ms)
  50%   3101
  66%   3176
  75%   3224
  80%   3263
  90%   3480
  95%   3905
  98%   4118
  99%   4591
 100%   8340 (longest request)
```