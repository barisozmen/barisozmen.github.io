# System Design Resources

System design of Twitter

<img src="https://user-images.githubusercontent.com/14996155/53670394-71176980-3c2f-11e9-8adc-1700bda93a5b.png" width="600">
source: https://www.infoq.com/presentations/Twitter-Timeline-Scalability


### Everything-in-it page
https://github.com/donnemartin/system-design-primer

### Interview solutions
   - How to design... 
      - Yelp: ([video](https://www.youtube.com/watch?v=tu6QKpV7GiI))
      - Twitter: ([video](https://www.youtube.com/watch?v=KmAyPUv9gOY&t=1214s)) ([video](https://www.youtube.com/watch?v=L7LtmfFYjc4))
      - Whatsapp: ([video](https://www.youtube.com/watch?v=5m0L0k8ZtEs)) ([blog](http://highscalability.com/blog/2014/2/26/the-whatsapp-architecture-facebook-bought-for-19-billion.html))
      - Uber/Lyft: ([video](https://www.youtube.com/watch?v=J3DY3Te3A_A))
      - Youtube: ([blog](https://www.geeksforgeeks.org/design-video-sharing-system-like-youtube/))
 - General:
    - Top 10 System Desing Questions ([hackernoon](https://hackernoon.com/top-10-system-design-interview-questions-for-software-engineers-8561290f0444))
    - A good [GitHub page](https://github.com/gorkemgenc/Large-Scale-Systems-Design-Explanation)

### Real-world examples (Tech Engineering pages)
Resource with many real-world system design explanations: http://highscalability.com/
 - Yelp: https://engineeringblog.yelp.com/2016/07/billions-of-messages-a-day-yelps-real-time-data-pipeline.html
 - Netflix: https://medium.com/netflix-techblog/evolution-of-the-netflix-data-pipeline-da246ca36905
 - AirBnb: https://medium.com/@airbnbeng
 - Facebook: 
    - [presto-interacting-with-petabytes-of-data-at-facebook](https://www.facebook.com/notes/facebook-engineering/presto-interacting-with-petabytes-of-data-at-facebook/10151786197628920/?s=keen-io)
    - [Paper: scaling memcached at facebook](https://cs.uwaterloo.ca/~brecht/courses/854-Emerging-2014/readings/key-value/fb-memcached-nsdi-2013.pdf)
 - Pinterest: [medium](https://medium.com/@Pinterest_Engineering/behind-the-pins-building-analytics-f7b508cdacab?s=hi-from-keen-io)
 - Twitter: 
     - [blog: handling five billion sessions a day–in real time](https://blog.twitter.com/engineering/en_us/a/2015/handling-five-billion-sessions-a-day-in-real-time.html)
     - [Twitter VP of Engineering talk: Platform infrastructure at Twitter](https://www.youtube.com/watch?v=FU7wrqsRj3o)
     - [video: Twitter timelines at scale](https://www.infoq.com/presentations/Twitter-Timeline-Scalability)
 - Uber: [engineering website](https://eng.uber.com/category/articles/architecture/)
 - Dropbox: [Video: How we've scaled dropbox](https://www.youtube.com/watch?v=PE4gwstWhmc)
 
### Step-by-step
 1. Requirements classification
 2. System interface definition
 3. Back-of-the-envelope estimation
 4. Defining data model
 5. High-level design
 6. Detailed design
 7. Identifying and resolving bottlenecks

### Very good course 
[Grokking the system design interview](https://www.educative.io/collection/5668639101419520/5649050225344512?affiliate_id=5082902844932096&utm_source=google&utm_medium=cpc&utm_campaign=platform2&utm_content=ad-1-dynamic&gclid=Cj0KCQiAzePjBRCRARIsAGkrSm6AItgy2HpLcFJO3hWDsWTQkbHufIYjtiHfoWi92AmvZRJSFMe9Ly0aAn8tEALw_wcB)

### Great book
[Distributed systems for fun and profit](http://book.mixu.net/distsys/single-page.html)

### Some terms
 - CAP Theorem ([video](https://www.youtube.com/watch?v=Jw1iFr4v58M), [blog](https://towardsdatascience.com/cap-theorem-and-distributed-database-management-systems-5c2be977950e))
    - Consistency, Availability, Partition tolerance

### Introduction to architecting systems for scale
https://lethain.com/introduction-to-architecting-systems-for-scale/
 - Load balancing
    - Smart clients
    - Hardware load balancers
    - Software load balancers
 - Caching
    - Application vs. Database caching
    - In-memory caches (e.g. [Memcached](http://memcached.org/), [Redis](https://redis.io/))
    - Content distribution networks
    - Cache invalidation
 - Off-line processing
    - Message queues
       - Tool: [RabbitMQ](http://www.rabbitmq.com/)
    - Scheduling periodic tasks
    - MapReduce
       - Tool: [Hadoop MapReduce](http://hadoop.apache.org/), [Hive](http://hive.apache.org/), [HBase](http://hbase.apache.org/)
    - Platform Layer
    
### HTTP requests 
https://www.codecademy.com/articles/http-requests
 - HTTP: Hypertext Transfer Protocol
 - TCP: Transmission Control Protocol
 - URL: Uniform Resource Locator
 - HTTP verbs:
     - GET — retrieve a specific resource (by id) or a collection of resources
     - POST — create a new resource
     - PUT — update a specific resource (by id)
     - DELETE — remove a specific resource by id
 - List of [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
 
### What is REST 
https://www.codecademy.com/articles/what-is-rest
 - REST: REpresentational State Transfer
 
### Data engineering pipeline 
with choices of technologies for each stage
<img width="992" alt="dataengpipeline" src="https://user-images.githubusercontent.com/14996155/54097102-db38b880-436b-11e9-8e00-24797e6a182f.png">

### CAP Theorem
<img width="332" alt="CAP Theorem. Source:https://robertgreiner.com/cap-theorem-revisited/" src="https://user-images.githubusercontent.com/14996155/75638829-b1168100-5be2-11ea-8ca8-473d8a4dc559.png">

In a distributed computer system, you can only support two of the following guarantees:

**Consistency** - Every read receives the most recent write or an error

**Availability** - Every request receives a response, without guarantee that it contains the most recent version of the information

**Partition** Tolerance - The system continues to operate despite arbitrary partitioning due to network failures
Networks aren't reliable, so you'll need to support partition tolerance. You'll need to make a software tradeoff between consistency and availability.
