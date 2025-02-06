# Usage

## Sum of requests

![Requests.png](Requests.png)

We are processing around **4.17 million** requests per month. More importantly, we can see sharp declines at night and over the weekends. Wildcat's current setup does not allow for scaling down during these lulls.

## Average Response Time

![ResponseTime.png](ResponseTime.png)

Our lowest average on any given day is **350.94ms** and our highest is **1,410ms**. Our average of all requests over the course of 30 days is **_1,110ms_**

To put things in perspective:

* Optimal range for user satisfaction(_"this app feels snappy!"_) is between **100-500ms**.

* Noticable Delay(_"Yeah, it has to think; this is fine"_) is between **500ms-1000ms**

* Tolerable Delay(_"Yeah, it's thinking hard; still fine but less fine"_) is between **1000-2000ms**

* Unacceptable Delay(_"Is this broken? Should I email support?"_) is anything **2000ms +**

## Maximum Memory Working Set

![MaxMemory.png](MaxMemory.png)

* Highest usage is **1.5Gb**

* Lowest usage is **0.24Gb**

## Average Memory Working Set

![AverageMemory.png](AverageMemory.png)

* **0.502Gb**

## Additional Notes

* An important thing to keep in mind during this comparison is the fact that App Services have roughly 10% of their memory being consumed by the underlying OS. In a containerized application, there is no underlying OS to consume memory.

* All of these statistics have been taken during the holidays; These numbers are likely much higher when fewer people are out on vacation