# Direct

 
 #### Going to DEV instance.
 
 ```
$ > httpd-2.4.23-x64-vc14\Apache24\bin\ab.exe -n 50000 -c 200 http://devuk.www.*.co.uk/
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
Server Hostname:        devuk.www.*.co.uk
Server Port:            80

Document Path:          /
Document Length:        33752 bytes

Concurrency Level:      200
Time taken for tests:   767.021 seconds
Complete requests:      50000
Failed requests:        0
Total transferred:      1707300000 bytes
HTML transferred:       1687600000 bytes
Requests per second:    65.19 [#/sec] (mean)
Time per request:       3068.084 [ms] (mean)
Time per request:       15.340 [ms] (mean, across all concurrent requests)
Transfer rate:          2173.72 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    2  13.6      1    3005
Processing:   250 3060 832.0   2756    9893
Waiting:      249 3053 831.2   2749    9888
Total:        251 3062 831.9   2758    9894

Percentage of the requests served within a certain time (ms)
  50%   2758
  66%   2888
  75%   3002
  80%   3104
  90%   4093
  95%   5251
  98%   5737
  99%   6155
 100%   9894 (longest request)
 ```
  