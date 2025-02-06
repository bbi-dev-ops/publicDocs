# Costs

In order to estimate costs, let's use the metrics from Current Wildcat as inputs for the [Azure Pricing Calculator](https://azure.microsoft.com/en-us/pricing/calculator/)

## Worst Case

Let's make the following assumptions that are informed by metrics we have available.

Monthly, this new app will:

* Recieve _**2x**_ requests: **8.3 million**

* Have **_2x_** as many concurrent users **500**

* Response times are **_2000ms_** per request

* We run the app hot, with every container having 4 vCPU and 8 GiB of memory

* At least one container is running 24/7 for frontend and backend

* We use the _"Pay as you go"_ consumption pricing plan:

![ACrequests.png](ACrequests.png)

![ActiveMonthlyAC.png](ActiveMonthlyAC.png)

![IdleTotalAC.png](IdleTotalAC.png)

Total possible monthly cost **_$191.62_**

This means with the most inefficient usage of resources, with twice as many users and requests, we would still be paying **_67.83% less_** per month for a radically more performant version of wildcat.

If we commit to a 3 year contract, this drops down to **_$157.05_** or **_73.59% less_**

In order for this new architecture to match current costs we would have to multiply this inefficiency 3 times over:

![absoluteWorstCase.png](absoluteWorstCase.png)

## Best Case

Let's be conservative and drop down to capacities more reflective of what Wildcat currently uses:

![Best.png](Best.png)

* Total monthly cost **_$94.62_** or **_84.09% less_** for equal or greater performance