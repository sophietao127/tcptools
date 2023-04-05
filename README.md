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
162.219.225.118

* How many hops were needed to reach the target? \
7

* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*AKAMAI-AP Akamai Technologies, Inc., SG*

* Identify the "class" of IP address for each major step in the trip \
Not know

**tracert: www.google.com:** 
* What was the target server's IP address? \
142.250.65.228

* How many hops were needed to reach the target? \
10

* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*AKAMAI-AP Akamai Technologies, Inc., SG* \
*AKAMAI-ASN1, NL* \
*GOOGLE, US* \

* Identify the "class" of IP address for each major step in the trip \
Not know

**tracert: www.microsoft.com:** 
* What was the target server's IP address? \
23.52.161.62
* How many hops were needed to reach the target? \
8
* Can you identify your ISP from the intermediate server DNS names? \
Yes, \
*AKAMAI-AP Akamai Technologies, Inc., SG*
*AKAMAI-ASN1, NL*

* Identify the "class" of IP address for each major step in the trip \
Not know
