# Direct

#### Going to NGINX node.
```
$ > httpd-2.4.23-x64-vc14\Apache24\bin\ab.exe -n 50000 -c 200 http://192.168.61.30/
This is ApacheBench, Version 2.3 <$Revision: 1748469 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 192.168.61.30 (be patient)
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
Server Hostname:        192.168.61.30
Server Port:            80

Document Path:          /
Document Length:        612 bytes

Concurrency Level:      200
Time taken for tests:   186.206 seconds
Complete requests:      50000
Failed requests:        0
Total transferred:      42250000 bytes
HTML transferred:       30600000 bytes
Requests per second:    268.52 [#/sec] (mean)
Time per request:       744.825 [ms] (mean)
Time per request:       3.724 [ms] (mean, across all concurrent requests)
Transfer rate:          221.58 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        0    4  84.8      1    3015
Processing:     2  741 3773.6    240   42292
Waiting:        2  539 3235.7    178   42291
Total:          3  744 3783.9    241   42293

Percentage of the requests served within a certain time (ms)
  50%    241
  66%    247
  75%    252
  80%    258
  90%    310
  95%    579
  98%   3260
  99%  27223
 100%  42293 (longest request)
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
  