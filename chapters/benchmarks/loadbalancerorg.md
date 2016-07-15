# Loadbalancer.org

 #### Going to NGINX Node
 
 
 ```
$> httpd-2.4.23-x64-vc14\Apache24\bin\ab.exe -n 50000 -c 200 http://192.168.61.27/
This is ApacheBench, Version 2.3 <$Revision: 1748469 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 192.168.61.27 (be patient)
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


Server Software:        nginx/1.10.1
Server Hostname:        192.168.61.27
Server Port:            80

Document Path:          /
Document Length:        612 bytes

Concurrency Level:      200
Time taken for tests:   189.846 seconds
Complete requests:      50000
Failed requests:        0
Total transferred:      45400000 bytes
HTML transferred:       30600000 bytes
Requests per second:    263.37 [#/sec] (mean)
Time per request:       759.383 [ms] (mean)
Time per request:       3.797 [ms] (mean, across all concurrent requests)
Transfer rate:          233.54 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    4  86.0      1    3036
Processing:     3  755 3558.9    249   39893
Waiting:        3  484 2761.7    163   33278
Total:          4  759 3568.6    251   39894

Percentage of the requests served within a certain time (ms)
  50%    251
  66%    256
  75%    261
  80%    266
  90%    292
  95%    496
  98%   6259
  99%  24313
 100%  39894 (longest request)
 ```


#### Going to `devuk.www.protolabs.co.uk`

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