# tcptools
## Using "Pings"
**Ping three popular websites**
1. What were the min/avg/max/stddev statistics for each?\
Test Performed from New York, NY \
Ping www.amazon.com: \
***1st**: rtt min/avg/max/mdev = 1.335/1.349/1.360/0.034ms;            0% packet loss;   IP: 173.223.58.31\
***2nd**: rtt min/avg/max/mdev = 1.620/1.620/1.620/0.000ms;            0% packet loss;   IP: 162.219.225.118\
***3rd**: rtt min/avg/max/mdev = 1.529/1.581/1.708/0.069ms;            0% packet loss;   IP: 13.226.31.9\
 Ping www.google.com: \
***1st**: rtt min/avg/max/mdev = 1.526/1.541/1.552/0.050ms;                    0% packet loss;   IP: 142.250.65.196\
***2nd**: rtt min/avg/max/mdev = 1.525/1.551/1.575/0.039ms;                    0% packet loss;   IP: 142.250.65.196\
***3rd**: rtt min/avg/max/mdev = 1.522/1.542/1.558/0.013ms;                    0% packet loss;   IP: 142.250.65.196\
 Ping www.microsoft.com: \
***1st**: rtt min/avg/max/mdev = 2.946/2.965/2.987/0.050ms;    0% packet loss;   IP: 23.200.197.152\
***2nd**: rtt min/avg/max/mdev = 2.956/2.982/3.002/0.037ms;    0% packet loss;   IP: 23.200.197.152\
***3rd**: rtt min/avg/max/mdev = 2.941/2.941/2.998/0.019ms;    0% packet loss;   IP: 23.200.197.152

2. Was there any packet loss on any of the pings?\
There was no any packet loss on any of the pings.

3. Did the IP address change for a given website between pings?\
For Amazon, yes, it did. \
For Google, no, it didn't. \
For Microsoft, no, it didn't

## Using "tracert"
**tracert: www.amazon.com:** 
* What was the target server's IP address? \
23.45.229.96

* How many hops were needed to reach the target? \
8

* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*seattle.compast.net*

* Identify the "class" of IP address for each major step in the trip
1. 10.0.0.1 - class A
2. 100.93.161.131 - class A
3. 24.153.85.89 - class A
4. 69.139.164.81 - class A
5. 69.139.164.81 - class A
6. 69.139.160.217 - class A
7. 69.139.160.217 - class A
8. 23.45.229.96 - class A

**tracert: www.google.com:** 
* What was the target server's IP address? \
172.217.14.196

* How many hops were needed to reach the target? \
12

* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*seattle.compast.net* 

* Identify the "class" of IP address for each major step in the trip
1. 10.0.0.1 - class A
2. 100.93.161.131 - class A
3. 24.153.85.89 - class A
4. 69.139.164.81 - class A
5. 69.139.164.81 - class A
6. 24.124.128.121 - class A
7. 24.124.128.121 - class A
8. 50.218.57.26 - class A
9. 108.170.245.107 - class A
10. 108.170.245.107 - class A
11. 108.170.245.124 - class A
12. 172.217.14.196 - class B

**tracert: www.microsoft.com:** 
* What was the target server's IP address? \
23.45.229.117
* How many hops were needed to reach the target? \
8
* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*seattle.compast.net*

* Identify the "class" of IP address for each major step in the trip
1. 10.0.0.1 - class A
2. 100.93.161.131 - class A
3. 24.153.85.89 - class A
4. 69.139.164.81 - class A
5. 69.139.164.81 - class A
6. 69.139.160.217 - class A
7. 69.139.160.217 - class A
8. 23.45.229.117 - class A

## Extra credit: Using packet-capture tools (2pts)
* Download/install Wireshark
* I tried to filter out any extraneous traffic so can only see the DHCP traffic, however, there is no any packert related to DHCP after filtering.
![test image1](dhcp.png)

## Extra credit: Insecure Web server (2pts)
* Navigate to http://150.230.36.255/
* Submit the login form with any email and password while capturing packets with Wireshark.
* Filter out any extraneous traffic so we see only the traffic to the server
* Take a screen shot of Wireshark showing the payload (email, password) you sent to the server
* Store the screen shot in the Github repo
![test image2](login.png)
