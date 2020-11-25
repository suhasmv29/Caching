# Caching
#### Cache

In computing, a data storage layer where a subset of data is stored, which operates at high-speed and is transient in nature is known as cache. Here, serving of data access requests are faster and better compared to accessing the data’s primary storage location every now and then. It makes the efficient reuse of previously retrieved or computed data. Starting from CPU to browser to any web app - all software rely on caching to a certain extent to provide blazing fast response. A latency of few milliseconds can lead to a loss of high revenue.

#### Benefits of Caching:
**Decreased network costs**: Caching of content can be done at various points in the network path between the consumer and origin. If the point is closer to the consumer, there will be no other network activity beyond the cache.

**Improved responsiveness**: Caching enables content to be retrieved faster as there is no need for an entire network round trip. Caches maintained close to the user, like the browser cache, can make this retrieval nearly instantaneous.

**Increased performance on the same hardware**: In the servers, where the content has originated, more performance can be squeezed from the same hardware.

**Availability of content during network interruptions**: With certain policies, caching can be used to serve content to end users, even when it may be unavailable for short time from the origin servers.

#### Key parameters:
Following are the key parameters based on which the caching strategy is chosen.
1. Business use-cases like high throughput, low latency
2. Data consistency threshold
3. Types of data that are stored like - Objects, Static data, Simple key-value pairs or In-memory data structures
4. Requirement of an in-process cache or shared cache in a single node or distributed cache for n number of nodes
5. Requirement of an open-source, commercial, or framework-provided solution
#### Types of caching

**Data Caching**:
Data Caching is best used for frequent access to data that does not change rapidly. This will help website or application load faster, giving users a better experience. It does this by avoiding extra trips to the DB (DataBase) to retrieve data sets that it knows has not changed.

The database is the bottle neck for almost all web application, so the fewer DB calls the better. Most DB solutions will also make an attempt to cache often used queries to reduce turnaround time.

It is a standard practice to clear any cache data after it has been altered. This way the Content Management System's (CMS) front-end will always have the most recent data and will not need to hit the database each time a user hits a page.

**Application/Output Caching**:
Most CMSs have built-in cache mechanisms. Application/Output caching can drastically reduce website load time and reduce server overhead. Different than Data Caching, which stores raw data sets, Application/Output Caching often utilizes server level caching techniques that cache raw HTML. It can be per page of data, parts of a page (headers/footers) or module data, but it is usually HTML markup.

**Distributed Caching**:
Most high volume systems like Google, YouTube, Amazon and many others use this technique. This approach allows the web servers to pull and store from distributed server’s memory. Once implemented, it allows the web server to simply serve pages and not have to worry about running out of memory. This allows the distributed cache to be made up of a cluster of cheaper machines only serving up memory. Once the cluster is set up, new machines can be added to the memory at any time without disrupting users.

#### Conclusion:
After doing analysis on caching approaches, for the project which is going through some performance and scaling issues, choosing a proper caching strategy by taking into consideration of the demands at the performance side will help to resolve the issue.

#### References:
* [https://aws.amazon.com/caching/](https://aws.amazon.com/caching/)
* [https://www.ironistic.com/four-major-caching-types-and-their-differences/](https://www.ironistic.com/four-major-caching-types-and-their-differences/)
* [https://www.fasthosts.co.uk/blog/caching-methods/](https://www.fasthosts.co.uk/blog/caching-methods/)
* [https://medium.com/datadriveninvestor/all-things-caching-use-cases-benefits-strategies-choosing-a-caching-technology-exploring-fa6c1f2e93aa](https://medium.com/datadriveninvestor/all-things-caching-use-cases-benefits-strategies-choosing-a-caching-technology-exploring-fa6c1f2e93aa)

