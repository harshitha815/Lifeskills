# Caching
## What is caching?
Caching is an approach to retrieve data that is being accessed frequently. It is used everywhere from your Household to the software industry. Just as we keep frequently used items like keys, remotes, or a book you’re currently reading within easy reach in our homes, caching stores frequently accessed data in a nearby storage location in your device. The main goal in both scenarios is to save time to make our everyday lives easier.
Cache in computing can be either hardware or software so that when it's accessed in the future, it can be retrieved faster. Since the cache is only a fraction of the main memory, it cannot store all the data. What gets stored depends on the caching algorithms that have been implemented.

## Caching- Algorithms
Least Recently Used (LRU) - It deletes the least recently used data items first.
Most Recently Used (MRU) - It deleted the most recently used data items first.
Pseudo-LRU - It deletes one of the least recently used data items.
Least Frequently Used(LFU) - It counts how frequently the data items are used and those that were used less often are deleted first.
First in First Out (FIFO)– Data items are added to a queue and deleted in the same order.
Random Replacement – It randomly selects a data item when the cache reaches maximum capacity and deletes it.

## Types of caching
There are various types of caching to improve the system’s performance.
1. Client-side caching: Data is cached on the client device to avoid delay. But it's important to refresh it, to avoid seeing old data.
Example: web page caching and In-app caching.
2. Server-side caching: Data is cached on the server to handle client requests efficiently.
Example: When a user visits a website, the server creates a copy of the webpage and stores it in the cache. When the user visits the website again, the cached copy is displayed instead of the server having to generate the page again
3. Database caching: Results of Database queries that are frequently used or accessed are stored in the cache to reduce repetitive database operations.
4. Distributed caching: Data is cached across multiple servers in a distributed system. This is ideal 
for applications that need to scale across multiple servers or different locations.
Example: E-commerce websites use distributed caching as it will ensure faster loading time for their consumers.
5. Content delivery network caching (CDN):  Data is cached in proxy servers that are closer to users than the original servers. When a user requests a web page the CDN sends the request to the nearest proxy server instead of the origin server which in turn reduces latency.
6. Memory caching: Temporarily stores data in the RAM for faster access.
7. Hybrid Caching: Combines multiple caching methods to improve performance.
Example: using CDN for static content and database caching for dynamic queries.
8. Predictive Caching:  Caches data that are likely to be accessed based on user behavior and patterns.
Example:  Google search anticipates the user’s needs and caches content to deliver results faster.
Google’s auto-complete suggests search queries based on user’s past queries.
9. Write-Through caching:  Data is written to both the cache and the primary storage at the same time when there is an update which ensures that the cache is always up-to-date.
Example: When a user updates any profile information it will be written to the cache and database at the same time to ensure consistent data.
10. Write-Back Caching:  Data is written to the cache first and written to the primary storage later. It improves performance as it reduces the number of writes to the database. Example: Logs are written to an in-memory cache immediately after they are generated. They are then written to the log storage system in batches.


## References: 
* https://www.geeksforgeeks.org/cache-eviction-policies-system-design/
* https://www.geeksforgeeks.org/what-is-the-caching-mechanism/
* https://youtu.be/6FyXURRVmR0?si=JjYShRPaa7C7CtR_
