##Xiao Luo
January 24, 2015


 
##Project 0

##1. MySQL:

keywords: relational

strength:

*  Easily installed and simple to get started. [1,2,3,4]
*  Supports a lot of SQL functionality that is expected from a RDBMS. [1]
*  Lots of advanced security features are built in MySQL. [2]
*  Popular and well industrialized.[4]
*  Scalable and Powerful. [2]
*  Fast. [2]
*  MySQL is support for atomic transactions. The ability to contain multiple operations within a transaction and roll back the whole thing as if it were a single operation. [2]
*  Memory factor: MySQL avoids memory leaks so that a the maximum storage for a single database can be 8 Tera byte. [3]
*  Security: MySQL take data safety a very important issue. Data are protected by encrypted passwords so that unauthorized access is almost impossible. Also data can be retrieved by backup, caching or log file so data loss is trivia.[3]

weakness:

*  Reliability issues.[2]
*  MySQL requires you to define your tables and columns before you can store anything, and every row in a table must have the same columns.
*  Might encounter sudden halt when dealing with too many operations simultaneously which means MySQL are not good at high concurrency operations. Concurrency read-write is still problematic.[2,4] 
*  Does not support SQL check constraints.[3]
*  Does not perform well on large size databases.[3]
*  Lots of useful functions are not build in core engine but are depends on add-ons.[4]

reference:

*  [1] http://www.neonrain.com/blog/mysql-vs-mongodb-relational-and-non-relational-databases
*  [2] https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
*  [3] http://gautambikash.hubpages.com/hub/Advantages-and-Disadvantages-of-MySQL
*  [4] https://www.datarealm.com/blog/five-advantages-disadvantages-of-mysql/
  
##  2. MongoDB:

Keywords: C++, NoSQL, in-memory database

strength:

*  Document Database: Great documents that reduce the need for joins and make polymorphism easier. Allow users to customize their own data type according to needs.[2,3]
*  High Performance: supports rich query expressions. Query commands using marks in JSON format, can easily search embedded objects and arrays in the document. Also MongoDB’s query optimizer will analysis the query expression and generate a efficient query plan based on it.[2-4]
*  High Availability: MongoDB database support server replication, namely support copying data between the master servers and other servers. The main objective is to provide redundant replication and automatic failover. [4]
*  Easy Scalabile: can do automatic sharding to distribute data on machines and dynamically balance the data size on machines.[2,3]
*  Rich query language: although MongoDB is using key-value storage, but it supports querying and indexing. [3]
*  Fast: Instead of keeping related data into multiple tables like relational database, MongoDB store related data together in documents so as to speed up queries. [2,3]
*  OS completely manages caching.[6]

weakness:

*  MongoDB does not support ACID transactions, but single operations are atomic.[6]
*  Since OS completely manages caching, it’s highly likely to cause OS releasing cached pages, as a result MongoDB may page to disk. And the size of database is limited by virtual memory of the operating system.[6]
*  MongoDB consumes too much disk space. [5]
*  Document size restriction: The max size of a MongoDB document is 16MB. [5]
*  Pagination using skips and limits have very bad performance. [5]

reference:

*  http://www.neonrain.com/blog/mysql-vs-mongodb-relational-and-non-relational-databases
*  https://www.mongodb.org/about/introduction/
*  http://www.zhihu.com/question/20059632
*  http://www.china-cloud.com/tushutuijian/20120209_9454_3.html
*  http://www.itexto.com.br/devkico/en/?p=44&utm_content=bufferac855&utm_source=buffer&utm_medium=twitter&utm_campaign=Buffer
*  http://www.quora.com/What-are-the-disadvantages-of-using-MongoDB-over-MySQL
*  http://docs.mongodb.org/manual/reference/limits/
*  http://www.acumensoftwaredesign.com/sql/strengths-and-weaknesses-of-nosql-vs-sql
 
##  3. HADOOP 

KeyWords: distributed, highly scalable storage platform, key-value

strength:

*  Cost effective [1]
*  With traditional method, massive data storage is very expensive so that many companies have to throw away lots of raw data. But Hadoop is designed as a scale-out architecture that can affordably store large sets of data. Hadoop is linear scaling in the ideal case.
*  Hadoop is open source software.
*  Flexible. Hadoop enables users to tap into various types of data so that it’s flexible in lots of purposes. [3]
*  Very high bandwidth to support MapReduce workloads [3,4]
*  HDFS can deliver data into the compute infrastructure at a huge data rate, which is often a requirement of big data workloads. HDFS can easily exceed 2 gigabits per second per computer into the map-reduce layer, on a very low cost shared network.
*  Distribute data and computation [2,3]
*  Fast. Due to Hadoop’s implementation schema, data is normally mapped to wherever it is located on a cluster and the tools for data processing are often on the same server as the data located, resulting in much faster processing speed.
*  Stable. The computation local to data prevents the network overload. This avoids failure and provides good fault tolerant in synchronous distributed systems. [2,3]
*  Flat scalability, specifically designed to have a very flat scalability curve that does not require large amount of refactoring. [1]
*  Resilient to failure[2-5]
*  Hadoop has excellent fault tolerance. When data is sent to an individual node, it is also replicated to other nodes in the cluster. So we can always have backup files when one is failed.
*  Hadoop’s tasks are independent so partial failure is easily handled.
*  Hadoop will automatically reassign failed tasks.
*  Easy to use: Hadoop has rather simple programming model, the end-user only need to write map-reduce tasks. [1]

weakness:

*  Rough manner: Because the software is still under active development and improvements are constantly being made. So not only the Hadoop Map-reduce and HDFS are rough in manner, but the stability of the version also worth noticing. [1]
*  Programming model is very restrictive for the lack of central data. [1]
*  When joining multiple dataset, usually the whole dataset is copied which is very inefficient.[1]
*  Does not support multi-user writes and cannot modify documents freely.
*  Still single master which requires care and may limit scaling. [1]
*  Security Concerns. [2]
*  Hadoop security model is disabled by default due to sheer complexity, so if people who manage the platform did not enable it, the data stored would be at huge risk. Also, hadoop miss encryption at the storage and network level.
*  Hadoop is written almost entirely in Java which is one of the most widely used but also controversial programming languages nowadays. Java has been heavily exploit by cyber-criminals, so that the use of hadoop may implicate in numerous security problems.
*  Not Fit for Small Data: Hadoop is designed for large capacity, so it lacks the ability to efficiently support random reads of small files. [2]

reference:

*  http://www.j2eebrain.com/java-J2ee-hadoop-advantages-and-disadvantages.html
*  http://www.bigdatacompanies.com/5-big-disadvantages-of-hadoop-for-big-data/
*  http://www.itproportal.com/2013/12/20/big-data-5-major-advantages-of-hadoop/
*  http://www.quora.com/What-are-the-advantages-of-Hadoop-over-distributed-RDBMS
*  http://www.slideshare.net/npinto/harvard-cs264-08b-mapreduce-and-hadoop
*  http://hortonworks.com/blog/thinking-about-the-hdfs-vs-other-storage-technologies/
  
##  4. Voldemort:

KeyWords: key-value hash table, column oriented

strength:

*  Highly scalable: [1]
*  Data is automatically partitioned so each server contains only a subset of the total data so the performance of write requests is improved as well as read. Because memory access is thousands of times faster than disk access, so the ratio of memory to data is the critical factor for accessing the performance of a storage system. By partitioning the data you increase this ratio by shrinking the data on each machine.
*  Increase capacity as traffic grows
*  Scale our with commodity hardware
*  As mentioned on the official website: “Provides tunable consistency (strict quorum or eventual consistency)”[2]
*  Data is under version control so as to maximize data accuracy when failure happens. [2]
*  Good single node performance: 10-20k operations per second. [2]
*  Support pluggable data placement so that users can be widely distributed but data transmission is still fast and data integrity is guaranteed. [2]
*  “Combines in-memory caching with the storage system so that a separate caching tier is not required. ”[2]
*  Make emulation for the storage layer possible since the layer is completely mockable. Development and test can be done without a real cluster or real storage system. [2,3]
*  Reads and writes scale horizontally [5]
*  Clusters can be expanded without the need to rebalance all data by using a transparent data partitioning method. [6]

weakness:

*  No complicated query filter [5]
*  All joint inquiry must be implemented in the code [5]
*  No structural foreign keys [5]
*  No triggers and views [5]

reference:

*  http://en.wikipedia.org/wiki/Voldemort_(distributed_data_store)
*  http://www.project-voldemort.com/voldemort/
*  http://blog.linkedin.com/2009/04/01/project-voldemort-part-ii-how-it-works/
*  http://www.54chen.com/document/dynamo-based-systems.html
*  http://wenku.it168.com/d_000492394.shtml
*  http://www.linuxlinks.com/article/20130414070552349/ProjectVoldemort.html
 
##  5. DynamoDB:

KeyWords: NoSQL

strength:

*  Fast, Consistent Performance: Using automatic data partitioning and SSD technologies to guarantee low latencies at any scale. [3]
*  Highly Scalable: Can self-define and update the request capacity using AWS Management Console or Amazon DynamoDB APIs.[3]
*  Flexible: Support both document and key-value data structure. [3]
*  Fine-grained Access Control: DynamoDB is integrated with AWS Identity and Access Management (IAM) which enable the user to authorize different security credentials to different user so as to control and manage their access to database. [3]
*  Fully Managed: DynamoDB help user dealing with tasks like hardware or software provisioning, software patching. With highly automatic design. [3]
*  There are several reasonable well working APIs, Ruby, Java etc that is integrated in the same Amazon APIs as the other Amazon services (the REST based API that these are built on leaves a fair bit to be desired, as does the documentation). [3]
*  Low cost: price is based on reserved capacity, calculation is simple and cost is predictable.[2]

weakness:

*   64KB limit on row size, 1MB limit no querying. [1]
*  Deployable only on AWS. [1]
*  Consistency comes with cost. Read capacity unit costs much more memory because it is based on strongly consistent read rather than eventually consistent read.[1]
*  DynamoDB has very limited querying function, especially on non-indexed data. Also, DynamoDB is unable to do complex queries.[1]
*  Do not have joins. [1]
*  Backup procedure is complicated and tedious comparing to RDS [1]
*  Do not support atomic transactions. [1]
*  Additional storage cost for each item. Amazon DynamoDB add 100 bytes of overhead to each item for indexing purpose. [1]
*  Once the read or write limit is hit, requests are denied for certain amount of time. [1]
*  Each write operation needs a read operation performed before that, this can be a disadvantage at situations like where there is read overhead and needs write to be very fast. [1]

reference:

*  http://www.slideshare.net/saniyakhalsa/dynamo-db-pros-and-cons
*  http://www.allthingsdistributed.com/2012/01/amazon-dynamodb.html
*  http://aws.amazon.com/dynamodb/details/
  
##  6. IBM Netezza:

strength:

*  Especially designed for data analysis, very cost-effective. [1]
*  compatible with oracle and mainstream BI tools. [1]
*  The system is easy to manage and maintain. [2]
*  Blade architecture, simple to extend. [1]
*  Use an elastic and fast way to replicate data from host to multiple target system. [1]
*  robust disaster recovery system. [2]
*  Excellent in the migration of large amounts of data, have negligible performance impact so as to ensure optimal bandwidth usage. [1]
*  Easy to backup the database, can implement partly recover or full recover. [1]
*  Using zone map technique, optimize data in the minimum data storage so as to improve query efficiency.[2]
*  SQL syntax is easier compared to other type of database. [3]

weakness:

*  Mix load control is bad. [3]
*  Performs portal weak security due to the weak SSL ciphers for encryption. [2]
*  When the data stored is largely modified, the performance will go down, need to manually groom the table. [1]
*  Disk backup data is pairwise, if both damaged then the data is hard to recover. [3]

reference:

*  http://wenku.baidu.com/view/a3edcbcfdd3383c4bb4cd2f5.html?re=view
*  http://www-03.ibm.com/software/products/zh/netezza-replication-services
*  http://xforce.iss.net/xforce/xfdb/90723
*  
##  7. SAP Sybase IQ:

strength:

*  Extremely high loading rate, integration of all available information. [1]
*  Massive capacity. [1]
*  Real-time and historical data integration. [2]
*  Sybase IQ provides a set of methods to support and expand a environment that arounds big data, for example, Sybase IQ support various monitoring tools and open tools, opened lots of interfaces for embedding tools like Hadoop, Mapreduce or even self-defined map-and-reduce function into Sybase IQ. This allows rapid analysis of massive volumes of data without the need to move data between systems. [1-4]
*  Sybase IQ is a column-based database, so it computes in a compressed format and the cost is relatively low compared to other types of database. The columnar architecture provides storage and access to time series data up to 100 times faster than row-based relational database. [5]

weakness:

*  Take more CPU load. [6]
*  IQ does not have row locks currently, so is not suitable for frequent data updates. [6]
*  Not suitable for real-time operations that includes deletion and updates. [6]

reference:

*  http://www.searchdatabase.com.cn/showcontent_61985.htm
*  http://www.itpub.net/thread-1501304-1-1.html
*  http://scn.sap.com/thread/3289509
*  http://www.sap.com/bin/sapcom/en_us/downloadasset.2013-01-jan-23-08.advantages-of-the-sap-real-time-data-platform-for-electronic-trading-pdf.html
*  http://leonid-gvirtz.typepad.com/blog/sybase-iq/
  
##  8. SAP HANA:

strength:

*  earlier period closing. [1]
*  better forecasting. [1] 
*  simulation of results or organizational changes. [1]
*  better insights into customer behaviour. [1]
*  real time sales and costs analysis in any fashion. [1]
*  flexibility to simulate organizational structures within the system. [2]
*  better service level in the customer facing applications. [3]
*  The in-memory technology enable users to explore and analyze data in real time from any data source. This technology also simplifies queries and models. Only need to persist calculation results when calculations are complex and contain external values.[2,5]
*  Accessing and indexing external data is available by using source-agnostic data access and integration services. [5]
*  Real-time analysis is available while business is happening. [2]
*  Can aggregating data without perturbing any on-going transactions.[5]
*  Business information is saved in Persistent Data Repository, and will be reconstituted if crash happens. [2]
*  Real-time Replication Service is available. [3]
*  Have SQL and MDX interfaces. [3]
*  Unified information modeling and design environment so that all data models are calculated virtually. [2]
*  Simplified Operations and Monitoring with the integration of basic HANA administration capabilities with the BW Admin Cockpit. [2]
*  supports parallel execution. [4]

weakness:

*  Currently only one big machine - which is not really perfect for HA scenarios
*  No PITR (point-in-time recovery - user errors -> deleting data accidentally)
*  HA scenarios are not covered by SAP - vendors will be responsible
*  no migration back to standard RDBMS, so SAP take your flexibility away

reference:

*  https://blogs.saphana.com/2014/08/29/the-benefits-of-the-business-suite-on-hana/
*  http://www.infinitesolutions.be/SAP-HANA-Features-and-Benefits
*  http://scn.sap.com/thread/2065611
*  http://www.dbbest.com/blog/sap-hana/
*  http://www.slideshare.net/ttrapp/hana-uni-halle
  
##  9. SAP Sybase ASE:

strength:

*  especially good at handling OLTP (On-Line Transaction Processing) workloads.
*  Extreme Compression that help reduce operational costs while increasing database capacity. Also save many time when accessing the data. [2]
*  High Performance. [2]
*  Ease of Administration. Great administration tools for monitoring. The cost of ownership can be reduced effectively by using storage, processing cycles and IT support resources. [2]
*  Efficient Disaster Recovery. Has integrated replication processes and automatic failure recovery to protect critical data. [2]
*  SAP Portfolio Integration. Have complete integration with the full portfolio of SAP products. Provide product synchronizing. [2]
  
weakness:

*  Rather newly emerging database that only limited experience is available.[3]
*  when workload change, administrator must change the configuration.[3]
*  reference:
*  http://sypron.nl/whatis_ase.html
*  http://klouddata.com/analytics/database-technology/sap-sybase-ase/key-features-and-benefits/
*  http://nntp-archive.sybase.com/nntp-archive/action/article/%3C3BCF3A30.61C17317@uchicago.edu%3E;jsessionid=F594D0B4F6467C93230C50AFBD219765
  
##  10. Oracle:

strength:

*  customized application. Customer can build up their own database that eliminate unnecessary features and only keep the features they need.
*  Data mining. Oracle database can find relationships between data better than human can do.
*  Run on all sorts of hardware, highly compatible.
*  Cost based query optimization.

weakness:

*  The program is not free and if been used on multiple computers, need to buy licenses for every computer.
*  Involves learning curve. Not simple to configure.
*  Oracle take up lots of memory and performance. 

reference:

*  http://www.ehow.com/info_12172600_list-pros-cons-oracle-database-11g.html
*  http://stackoverflow.com/questions/1856414/cons-of-oracle-database
*  http://www.databasejournal.com/features/which-database-is-best-for-you.html
  
##  11. Oracle CEP:

strength:

*  Will benefit from having a single library of message.
*  Oracles’s data guard is one of the best solution to database clone and disaster recovery.
*  Excel at situation that need indexing or processing data when massive data is stored at back-end database because read/writes operations will not interrupt each other and data remain consistent during the process.
*  Great tool for supporting  JAVA.

weakness:

*  Need more multi-dimentinal data cube to store data which cost more space and money.

reference:

*  http://blog.ventanaresearch.com/2010/11/28/advantages-and-challenges-of-in-memory-databases-and-processing/
*  http://searchsoa.techtarget.com/tip/Complex-Event-Processing-CEP-with-SOA-creates-business-benefits
*  http://searchsoa.techtarget.com/feature/Complex-event-processing-boosts-agility-to-create-competitive-advantage
*  http://tech.it168.com/a2010/0325/865/000000865624_all.shtml
*  
## 12. Google Cloud SQL:

strength:

*  High Availability. Cloud-based SQL database reduce the possibility of going down when meet high traffic and sales times, provide protection against this with high availability technology and distributed resources. [2]
*  cheaper for most types of work loads. [2]
*  scales massively for reads and writes. [2]
*  Higher Productivity: updates are distributed efficiently. [2]
*  Less Disruption is Caused When Users Adopt New Functionality: Instead of large disruptive batches of change, manageable improvements is delivered gradually. [2]
*  Employees can have access to information from anywhere in the world through Google cloud regardless of the devices. [2]
*  Quick Collaboration. [2]
*  Security: Google pays a lot on security issues to protect users’ data. [2]
*  Less Data has to be stored on Vulnerable Devices: they are on the cloud. [2]
*  Customers get Higher Uptime and Reliability: If the optimal data center is not available at the moment, the connection will automatically established to the next available data center without any delay. [2]
*  Control and Flexibility Available to Users:  Data can be easily added and removed from the cloud based on customer needs. [1,2]

weakness:

*  Limited to Python/Java environment [3]
*  Limits the maximum rows returned from an entity get to 1000 rows per datastore call. [1]
*  vendor dependency - relatively hard to port application to other platform. [4]

reference:

*  http://www.vi.net/blog/2013/07/five-advantages-of-running-a-sql-server-database-in-a-cloud-environment-or-virtual-machine/
*  http://www.netsolutionsindia.com/blog/what-is-google-cloud-its-advantages-and-why-you-should-adopt-it/
*  http://www.quora.com/What-are-the-advantages-and-disadvantages-of-using-Google-Cloud-Datastore-vs-Google-Cloud-SQL
*  http://programmers.stackexchange.com/questions/181063/google-app-engine-what-are-the-advantages-and-limitations

##  13. Cassandra:

strength:

*  Low write latency with respect to small to medium write sizes [1]
*  Linear write scalability [1]
*  Fault-tolerance across geographic locations. [2]
*  High-scale out, high-throughput transactional system. [3]
*  Tunable consistency and support for replication [3]
*  Atomic, scripted updates. [2]

weakness:

*  Failed operations may leave changes. [3]
*  Searching is very complicated. [3]
*  Bad at the consistent indexes on values as well as the consistent read/write latency of heavy load. [4]

reference:

*  http://grokbase.com/t/cassandra/user/1474dnp0tn/cassandra-use-cases-strengths-weakness
*  http://www.ibm.com/developerworks/library/os-apache-cassandra/
*  http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
*  http://www.quora.com/What-are-the-main-disadvantages-of-using-cassandra-what-are-the-scenarios-where-cassandra-should-not-be-my-first-selection

##  14. Redis:

keyword: in-memory

strength:

*  Exceptionally Fast: can perform 110000 SETs per second, about 81000 GETs per second.
*  Support rich data types: Redis natively support most of the datatypes that most developers already know like list, set, sorted set, hashes.
*  Operations are atomic which ensures that if two clients concurrently access Redis server will get the updated value.
*  Multiutility tool: can be used in a number of use cases like caching, messaging-queues.
*  Replication possible[2].
*  Lots of datasturcture available with realm of key-value.[2]

weakness:

*  Memory only, so all data must fit in memory, cannot manage more data than what you have in your memory[2,3]
*  not distributed yet.[2]
*  No query language and no support for a relational algebra.[3]
*  Only offers basic security at the instance level.[3]
*  Persistency affects performance. Redis uses memory dump to create a persistency snapshot, but this requires some linux kernel tweaking to avoid performance degradation while Redis server process is forking.[3,4]
*  Memory fragmentation issues: writing and deleting huge amours of data may result in performance degradation.[4]

reference:

*  http://java.dzone.com/articles/introduction-to-redis-in-memory-key-value-datastore
*  http://www.quora.com/What-are-the-advantages-and-disadvantages-of-using-MongoDB-vs-CouchDB-vs-Cassandra-vs-Redis
*  http://stackoverflow.com/questions/10906246/what-is-the-disadvantage-of-just-using-redis-instead-of-an-rdbms
*  http://www.quora.com/What-are-the-disadvantages-of-Redis
  
##  15. Riak:

strength:

*  works great in the situation that data does not fit on a single server but demands a distributed database. [1]
*  Great resilience and tolerance to network partitions and hardware failures which would significantly disrupt most database. [1]
*  Predictable latency, for its basic operation (eg,. read, write and delete) do not involve complex data joins or locks. [1]
*  Minimizing the cost of scale. [2]

weakness:

*  Maybe overkill for small databases. [1]
*  data have to be stored in the format of key-value pair. [1]
*  Performs bad on applications that demands a high query load expect for key-value lookups. [1]
*  Does not support strictly consistent operations. [2]
*  Does not support model of traditional relational systems. [2]
*  
reference:

*  http://docs.basho.com/riak/latest/theory/why-riak/
*  http://basho.com/assets/RelationaltoRiakDEC.pdf
  
##  16. HP Vertica:

strength: 

*  fast on large amount of data. [1]
*  good performance on clustering and commodity hardware. [2]
*  column-based storage structure which improves the ability to deal with continuous records. But it adds a separate cost in normal operations which is the updates and deletion for single records.[2] 
*  It’s compressed so as to save storage cost and IO bandwidth cost. [2]
*  Does not have sharing architecture which reduces the competition between systems for shared resources. [2,3]
*  Mixed data storage mode, when doing insertion, implementing high concurrency operation on both insert and write by the principle of write priority. [2,3]
*  Automated database structure design tool for multi-node cluster system. All data will be store on more than one node, namely k-safety, in an attempt to avoids the loss cost by single node failure. [3]

weakness:

*  future competition is weak [1]
*  high loan rates are possible [2]
*  tax structure [2]
*  investments in research and development is not enough [2]
*  cost a lot [2]

reference:

*  http://stackoverflow.com/questions/8987727/advantages-of-databases-like-greenplum-or-vertica-compared-to-mongodb-or-cassand
*  http://wenku.baidu.com/view/85b665c258f5f61fb7366667
*  http://swot.advisorgate.com/swot-h/18568-swot-analysis-hp-vertica.html
  
##  17. MapR:

keywords: c++, hadoop

strength: 

*  Removes the single point failure that bothers Apache Hadoop distributed system (HDFS) by using distributed namenode architecture. [1]
*  high availability. [1]
*  Fast recovery from failure, satisfies the need for big data applications that cannot afford to lose data. [2]
*  architecture is 100% binary compatible with the Apache Hadoop distributed file system so as to ensure plug-and-play compatibility and no vendor lock-in. [2]
*  Does not require separate clusters for multiple applications, is able to process both distributed files and database tables in one unified layer so that it support both operational and analytic apps on one cluster. [2]
*  Open source, no license cost. [3]
*  MapR can handle data while it is changing using an ANSI-SQL query engine. It also support for nested and schema-less storage. [6]
*  MapR has an ultra-strong security system, so everything is encrypted. [6]

weakness:

*  The mutable data adds complexity to the system design. [4]
*  Does not perform well on huge clusters. [5]

reference:

*  https://www.mapr.com/why-hadoop/why-mapr
*  http://technews.tmcnet.com/channels/hadoop/articles/319064-advantages-mapr-technologies-hadoop-distribution.htm
*  http://stackoverflow.com/questions/15079701/what-are-disadvantages-of-the-hadoop-distribution-mapr-compared-to-cloudera-and
*  http://wikibon.org/wiki/v/MapR_Hadoop_Strategy_Stresses_Performance,_Availability_and_API_Compatibility_Over_Open_Source_Code
*  http://siliconangle.com/blog/2013/06/27/mapr-vision-for-hadoop-one-platform-for-big-data-hadoopsummit/tomer-shiran/
*  http://www.forbes.com/sites/danwoods/2014/09/29/can-mapr-keep-ahead-of-hadoop-competitors/
  
##18. Azure DocumentDB:

keywords: microsoft, noSQL,

strength: 

*  Rich query and transactions over schema-free JSON data. Automatically indexes all JSON documents added to the database with a highly concurrent, lock free, log structured indexing technology, so that SQL syntax can be used to query them. [1]
*  Delivers reliable and configurable performance. [1]
*  Enables rapid development, in other words, programming against DocumentDB is simple and does not require custom encoding or extensions to JSON or JavaScript. [1]
*  Offers four distinct consistency levels: strong, bounded-staleness, session and eventual. [2]
*  Helped users to manage virtual machines, deploy and configure software, as well as deal with complex data-tier upgrades. Database is automatically backed up so as to be protected against regional failures. [2]
*  Elastically scalable throughput and storage. [2]

weakness:

*  only support .Net, Javascript and python as programming language. [3,4]
*  Currently does not allow join and combine. Does not allow queries to operate on multiple databases. [5]

reference:

*  http://azure.microsoft.com/en-us/services/documentdb/
*  http://azure.microsoft.com/en-us/documentation/articles/documentdb-introduction/
*  http://db-engines.com/en/system/Cassandra%3BElasticsearch%3BMicrosoft+Azure+DocumentDB
*  http://geekswithblogs.net/hroggero/archive/2014/09/11/documentdb-vs-azure-sql-vs-azure-table.aspx
*  https://social.msdn.microsoft.com/Forums/sqlserver/en-US/7a4d7874-a5c9-4aab-a5f7-5a9569afc224/what-are-the-azure-document-db-limitations-how-is-it-better-than-azure-sql?forum=AzureDocumentDB
  
##  19. Azure SQL Database:

keywords: microsoft, relational database-as-a-service

strength: 

*  offer relational storage which provides a schema and a strongly typed data store. [1]
*  streamline business continuity for critical applications, no physical administration. [1,2]
*  Support various of familiar tools and platforms so as to make user easier to take advantage of multiple resources and fasten their tasks. [1]
*  Enable security and compliance-related tasks. [1]
*  Being offered in different service tiers to support light-weight to heavy-weight database workloads, this makes Azure SQL a scalable service plan for multiple needs and budges, suitable for both big and small business users. [2]
*  Elasticity. Applications written for multiple databases can be scaled out with Azure by adding instances as needed. [1,2]
*  Support lots of non-Microsoft technologies. [1]
*  Have sync and migration tools. [2]

weakness:

*  Only implements a subset of T-SQL, especially the users cannot run agented jobs. [3]
*  User data is not hosted locally, the only way to get data to an Azure instance is to upload it or sync it across network. [4]
*  Azure SQL has hard-wired limitations on usage and will throttle or disconnect database connections under heavy loads. [4]
*  SQL reporting is also charged. And there might be charges for outbound data. [4]
*  Limited backup. [4]

reference:

*  http://azure.microsoft.com/en-us/services/sql-database/
*  http://searchsqlserver.techtarget.com/feature/The-pros-of-Windows-Azure-SQL-Database
*  http://searchsqlserver.techtarget.com/feature/Why-you-should-think-twice-about-Windows-Azure-SQL-Database
*  http://stackoverflow.com/questions/6560427/choosing-the-right-database-on-cloud-azure-sql

##  20. BerkeleyDB:

keywords: oracle, key-value, not relational

strength: 

*  open-source embedded database. [1]
*  directly connected to the application, so BerkeleyDB and the application are running in the same memory space which can avoid interprocess communications. Low-level services (e.g., locking, transactions logging) can be transparently implemented by the library. [1]
*  highly portable. Can run on top of almost all UNIX and Linux systems, also support windows and other embedded real-time operating system. [1]
*  Library is very compact. Support concurrent operations and allowing thousands of users operate in the same database in the field of high-end servers. Does not take up too many memory space. [1]

weakness:

*  mutex may be held for many thousands of instructions, limiting the degree of parallelism in the application if it is lock intensive. And limit library flexibility as well. [4,5]
*  BerkeleyDB B tree access method will require repeated buffer pool lookups when traversing an index rather than memory indirections which is cheaper. [3]

reference:

*  http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/overview/index.html
*  https://web.stanford.edu/class/cs276a/projects/docs/berkeleydb/ref/build_vxworks/introae.html
*  ftp://ftp.research.microsoft.com/pub/debull/A07sept/seltzer.pdf
*  http://www.databaseskill.com/449542/
*  http://www.oracle.com/technetwork/articles/cloudcomp/berkeleydb-nosql-323570.html
*  http://www.aosabook.org/en/bdb.html
  
##  21. SQLite:

keywords: relational, 

strength: 

*  File based: The entire database is a single file on the disk, so it is extremely portable. [1]
*  Standards-aware: SQLite uses SQL, although there are some features (e.g., RIGHT OUTER JOIN or FOR EACH STATEMENT) is not available, there are also additional features been added. [1]
*  Great for developing and testing because SQLite has rich feature bases, which provide convenience to development , also it is linked to C based library. [1]
*  No need to be “installed ” before it is used. [1]
*  The process that wants to access the database reads and writes directly from the database files on disk rather than using some kind of interprocess communications (typically TCP/IP). [2]

weakness:

*  SQLite does not have high level multi-client concurrency function support, so when need to manage the connections with set access privileges to database and tables, SQLite is not a good choice. [1]
*  Lack of possibility to tinker with for additional performance. [1]
*  When write volumes is high, SQLite does not perform very well. [1]
*  Slow: locks whole file for writing and no caching mechanism of it’s own. [2]

reference:

*  https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
*  https://www.sqlite.org/different.html
  
##  22. PostgreSQL:

keywords: relational, 

strength: 

*  Open-source and free. [1]
*  strong community: PostgreSQL can be accessed through knowledge-bases and Q&A site 24/7 for free. [1]
*  strong third party support: PostgreSQL is merged with many extremely useful and open-source third-party tools for designing, managing. [1]
*  Extensible: Able to extend the stored procedures using programmatically. [1]
*  Objective: with support for nesting and more. [1]
*  Perform better than other tools when reliability and data integrity are first priority concerns. [1]
*  Its multi-value fields (e.g, arrays, nested tables) reduces the need for joins and increase the performance of storing as well as retrieving “multi-dimensional” data structure. [2]
*  has class based inheritance between tables so that tables could inherit common properties. [2]
*  has a very rich data type systems and allows user-defined data types and composite data types. [2]

weakness:

*  Performance: For simple read-heavy operations, PostgreSQL might be over perform and might appear less performant than other database. [1]
*  Not very popular. And this may influence it’s technical support behind the scene.[2]
*  Replication is not as well implemented. [3]
*  Host: For the reasons mentioned above, it’s harder to find a host or server supplier to provide instances on managing PostgreSQL. [1]
*  no default parameteres in plpgsql. [3]
*  no support built into plpgsql to create web-based procedures. [3]

reference:

*  https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems
*  http://www.quora.com/What-are-pros-and-cons-of-PostgreSQL-and-MySQL
*  http://forums.devshed.com/postgresql-help-21/advantages-disadvantages-postgresql-106805.html
 
##  23. Informix:

keywords: IBM

strength: 

*  unleashes new capabilities, be able to combine unstructured and structured data. Support both relational and non-relational data. [1]
*  Offers the industry’s most comprehensive set of high availability hardware with Informix Flexible Grid. Upgrades and maintenance can be scheduled without any downtime and without having to use temporary hardware or clone to databases and applications. [1]
*  Provides easy, graphical tools that increase developer productivity. Provide increased support for standard SQL and enable more open source applications. [1]
*  Provide a time-series feature which provides unprecedented performance and scalability to applications. Also offers  a built-in spatial feature to enable location-based applications. [1]
*  Automatically senses and responds to changes without human or programmatic intervention. it’s self-maintaining, self-configuring, self-healing. [1]
*  Enhanced security speeds time to compliance. [1]
*  Fast.
*  Reduce risk for sharing data on private cloud and save cost for enterprise deployment. [1]

weakness:

*  Less management tools than other product. [4]
*  Fault tolerance mechanics is rather simple.[3]

reference:

*  http://www-01.ibm.com/software/data/informix/features.html
*  http://www.answers.com/Q/What_is_the_advantages_of_informix_than_oracle
*  http://eecatalog.com/ibminfo/files/2010/11/Cost-Benefit-Case-for-IBM-Informix-Compared-to-Microsoft-SQL-Server-for-Midsize-Organizations.pdf
*  http://www.informixchina.net/home/space.php?uid=95&do=blog&id=456

##  24. CouchDB:

keywords: NoSQL, document-oriented database

strength: 

*  no read locks, so CouchDB has better performance when been concurrent used by multiple users. Changes are always appended to the end of the database file. [1]
*  Supports trivial hot back-ups. “Users can make a point-in-time backup of a CouchDB database file with cp command while CouchDB is running. ”[1]
*  Documents can be in any index and number of times. [1]
*  Replication is easy and bidirectional. [2]
*  Save space by leaving empty fields in documents. [2]
*  Fast and agile schema updates. [3]
*  MapReduce queries in a turing complete language. [2,3]
*  Replication is easy and fast. Supports fast peer-to-peer replication and sync between remote CouchDB databases. [3]

weakness:

*  Trade disk space VS speed: Because change are appended to end of file, the actual database file can grow huge. [3]
*  Not good at dealing with relational data. [4]
*  Data warehouse. Temporary views in CouchDB on large datasets are slow, because it cannot use formal indexing technic. [4]
*  Does not support transactions. [3]
*  No built in full text search. [5]
*  Replications on large databases may fail. [5]
*  “only” eventual consistency. [5]

reference:

*  http://willconant.com/posts/2013-06-02/4-good-things-about-couchdb
*  http://stackoverflow.com/questions/644695/what-are-the-advantages-of-couchdb-vs-an-rdbms
*  http://www.quora.com/How-does-MongoDB-compare-to-CouchDB-What-are-the-advantages-and-disadvantages-of-each
*  http://eflorenzano.com/blog/2008/11/23/why-couchdb-sucks/
*  http://stackoverflow.com/questions/7858699/disadvantages-of-couchdb
  
##  25. Elasticsearch:

keywords: document-oriented, NoSQL, Lucene

strength: 

*  Elasticsearch is distributed. No separate project required. Replicas are near real-time. [1]
*  Fully supports the near real-time search of Apache Lucene. [1]
*  Using Gateway which makes full backups easier. [1]
*  Schema free and Document oriented. [1]
*  Can do cluster on search. [2]
*  Easy to install. [2]

weakness:

*  Security: ElasticSearch does not provide any functions related to authentication or access control. [2]
*  Transactions: does not support transactions or processing on data manipulation. [2]
*  Durability: backups and durability are not as high priority as in other databases. [2]
*  ElasticSearch is still relatively new and needed to be further improved. Its client libraries and third party tools are not mature. [3]
*  Commands for searching data are not suited to “large” scans of data and advanced computation on database side. [3]
*  It may lose write. [4]

reference:

*  http://java.dzone.com/articles/introduction-elasticsearch
*  http://www.quora.com/Why-should-I-NOT-use-ElasticSearch-as-my-primary-datastore
*  http://digiter.diandian.com/post/2012-11-05/40042547383
*  http://blog.winwu.today/2014/07/elasticsearch.html
  
##  26. Firebird:

keywords:

strength:

*  multi-generation architecture: readers do not lock writers. Firebird is designed to provide for many clients accessing a single database at the same time. client applications can have active connections to several databases simultaneously. [1]
*  Light and easy to install. [1]
*  rich SQL: high compatibility with ANSI SQL, common table expressions, flexible transactions management etc. [2]
*  Trace API: This API can be used to perform a number of security and management tasks programmatically, can implement real-time monitoring and SQL debugging. [2]
*  Security: Firebird maintains a security database storing user names and encrypted passwords. Using windows trusted authentication. [2]
*  Transactions: Firebird client applications have full control over the starting, committing and rolling back of transactions. [2]
*  Multigenerational architecture: multiple versions of each data row can be created and stored as necessary if a transaction modifies the row. [3]
*  Optimistic row-level locking: User-initiated locking is unnecessary, engine will lock a row to there transactions only when a transaction signals that it is ready to update it. [3]
*  Database administration: been abundantly supported by open source, freeware and commercial GUI database administration utilities. [1,3]
*  Firebird have two command-line backup or restore tools, both of them does not require exclusive access to the database, so clients can remain connected and perform operations when the database is doing backup. [1]
*  Each database is located in one independent file, that can be located anywhere on the disk.

weakness:

*  Community project, without the official producer support. Possible problems must be solved individually by the user. Related to this fact, there is some minor portion of slightly obsolete documentation. [3]
*  Documentation is poor. [4]

reference:

*  http://www.firebirdsql.org/manual/ufb-about-features.html
*  http://www.slideshare.net/mindthebird/why-firebird-fact-for-decision-makers
*  http://www.promotic.eu/en/pmdoc/Subsystems/Db/FireBird/FireBird.htm
*  http://www.dreamincode.net/forums/topic/354458-advantages-and-disadvantages-of-firebirdsgl/
  
##  27. Hortonworks:

keywords: Hadoop

strength:

*  Completely open-source, actually the only open Hadoop data platform available. [1]
*  Using linear scale storage. Can compute through a wide range of access methods (e.g., batch, interactive, real-time, search and streaming). [1]
*  Integrates with and augments customers existing applications and systems so that users can create their works with only minimal change to existing data architectures and skillsets. [1]
*  Access data from a variety of engines. [2]
*  Load and manage data according to policy. [2]
*  System has multi-layer security. Important features like authentication, authorization, accountability are all included and well implemented in the system to guarantee a secure information delivery. [1]

weakness:

*  The whole file must be read for every computational process because by its nature there are no predefined data schema or indexes. [3]
*  Have bad performance when many small files are stored in the distributed file system. Because if only few nodes are needed, the cost of managing the distribution of files and systems is not economic.[3]

reference:

*  http://hortonworks.com/hdp/
*  http://hortonworks.com/wp-content/uploads/2014/02/Hortonworks_Solution_Overview_VMware_01_27_2014-1.pdf
*  http://www.sapns2.com/files/white-paper/SAP%20NS2%20paper%20on%20HADOOP%20-%2007.06.12.pdf
  
##  28. Apache S4:

keywords: yahoo

strength:

*  “Fill the gap between complex proprietary systems and batch-oriented open source computing platform.” [2]
*  “Decentralized: all nodes are symmetric with no centralized service and no single point of failure which greatly simplifies deployments and cluster configuration changes.” [2]
*  “Scalable: throughput increases linearly as additional nodes are added to the cluster. There is no predefined limit on the number of nodes that can be supported.” [2]
*  Extensible: applications can easily be written and deployed using a simple API. Building blocks of the platform can be replaced by custom implementations. [2]
*  “S4 hides all cluster management tasks using a communication layer built on the top of a distributed, open-source coordination service for distributed applications.” [2]
*  “High fault-tolerance: when server in the cluster fails, a stand-by server is automatically activated to take over the tasks. Checkpointing and recovery minimize state loss called “zookeeper”.” [2]

weakness:

*  Failover: when running nodes crash, the PE data on the current node can not implement failover. [3]
*  Persist: current supporting method is too simple. For future improvement S4 need to consider persistent network (similar to nfs, distributed file systems). [3]
*  Communication: only support udp protocol. [3]
*  Deploy: not automatically deploy, can not support zero deploy mode of apps. [3]
*  reference:
*  http://greeensy.github.io/Big-Data/
*  http://incubator.apache.org/s4/
*  http://blog.csdn.net/derekjiang/article/details/7203201
  
##  29. Apache Storm:

keywords: twitter, yelp, taobao, baidu, yahoo

strength:

*  Better fault-tolerance solution. Guarantees no data loss by the acker.[2,3]
*  Allows user to configure task’s parallel hints and the number of the workers to execute topologies.[2]
*  Fast: benchmarked as processing one million 100 byte messages per second per node.[3]
*  Scalable: [3]
*  Reliable: Storm guarantees that each unit of data (tuple) will be processed at least once or exactly once. Messages are only replayed when there are failures.[3]
*  Easy to operate.[3]

weakness:

*  Does not support multi-core processing load. [4] 
*  Perform worse than some other systems when there is huge load at front end, may result in large increase of apache processes thereby denying to continue working. [4]

reference:

*  http://greeensy.github.io/Big-Data/
*  https://groups.google.com/forum/#!topic/storm-user/3DG072eol2Y
*  http://hortonworks.com/hadoop/storm/
*  http://study.byoou.com/Apache%E4%B8%8ENginx%E7%9A%84%E4%BC%98%E7%BC%BA%E7%82%B9%E6%AF%94%E8%BE%83.html 
*  http://www.infoq.com/presentations/Storm
*  http://stackoverflow.com/questions/11250028/twitter-storm-compared-to-hadoop
  
##  30. Hbase:

keywords: Apache, hadoop, NOSQL

strength:

*  free open source software.
*  Fault tolerant storage for large quantities of data. when a node fails, Hbase automatically recovers the writes in progress and edits that have not been flushed. [1,2]
*  Flexible data model [3]
*  Easy Java API as well as Thrift, or REST gateway APIs [2]
*  Near real-time lookups, Hbase is able to provide random, real-time access to its data by utilizing the configuration bloom filters, block caches etc. [1,2]
*  Atomic and strongly consistent row-level operations [1]
*  Automatic sharing and lad balancing of tables [1]
*  Metrics exports via File and Ganglia plugins [2]
*  High availability through automatic failover [3]
*  In-memory caching via block cache and bloom filters [1]
*  Server side processing via filters and co-processors [1]
*  Replication across the data center [2]
*  Strong Consistency: Have a strong consistency on reads and writes. A single server in an HBase cluster is responsible for a subset of data with atomic row operations. [2]
*  Dynamic increasing columns, and if the column is empty then no data will be stored so as to save more space. [7]

weakness:

*  Requires an additional request to NameNode in order to find a DataNode strong required block.[5]
*  Data should be transferred from the DataNdoe to RegionServer on reads in some cases.[5]
*  Lacks many of the features of RDBMS, does not support SQL. [5,6]
*  Can not establish second level indexing.
*  When region is compacting or splitting, there might be short period of read-write stuck.
*  Security: as long as the IP and port of ZK is known, Hbase can be easily visited without any authentication and authorization.
*  Does not support master server change when failure, so if the master break down, the whole storage system dies. [7]

reference:

*  https://blogs.apache.org/hbase/
*  http://hortonworks.com/hadoop/hbase/
*  http://blog.credera.com/technology-insights/java/apache-hbase-explained-5-minutes-less/
*  http://blog.cloudera.com/blog/2011/04/hbase-dos-and-donts/
*  http://www.slideshare.net/DmitriBabaev1/cassnadra-vs-hbase
*  http://zhan.renren.com/tag?value=hbase
*  http://f.dataguru.cn/thread-206547-1-1.html

##  31. Teradata:

keywords: relational

strength:

*  Linearly scalable: database capacity can be enlarged simply by adding nodes to existing database. [1]
*  Extensive parallel processing: can handle multiple ad-hoc requests and perform well on concurrency issues. [1]
*  Shared nothing architecture: very high fault tolerance and data protection. [1]
*  Low total cost of ownership: easy to setup, maintain and administrate. Very low disk to data ratio. [2,4]
*  Suitable of extremely large data set. [3]
*  Mixed workload performance, ability to keep data current and handle different types of queries. [4]
*  In-database advanced analytics, including geospatial, temporal, data mining and modeling. [4]
*  Partition Primary Index: rows are distributed based on different partitions so their retrieve is faster. This also reduces the overhead of scanning complete table. [5]

weakness:

*  not suitable for small transaction OLTP databases. [1]
*  Poor tools. [3]
*  With the use of partition primary index, a primary index access can be degraded if the partition column is not part of the primary index. When doing join to non-partitioned table with partition primary index, the join may be degraded. And primary index can not be defined UNIQUE when the column is not part of primary index. [5]

reference:

*  http://forums.teradata.com/forum/enterprise/advantages-of-teradata-over-other-databases
*  http://softdocs.blogspot.com/2011/03/teradatas-advantages.html
*  http://server.dzone.com/articles/oracle-vs-teradata-vs-hadoop-1
*  http://www.slideshare.net/teradata/teradata-database-14
*  http://www.teradatatech.com/?p=1010
  
##  32. DB2:

keywords: relational

strength:

*  Powerful structure Query language than SQL offer. Provide lots of features that MySQL does not support such as object tables and Java method support. SQL allows direct access to data via DB2 interface. [1]
*  Multiple platform support: support AIX, HP-UX, Linux, Windows, Sun. [1]
*  Self-Tuning Memory Management. [1]
*  Have strong IBM support, is a rather mature technology. [1]
*  self-configuring, self-healing, self-tuning, self-protecting. [2]
*  lower upfront license cost and lower total cost of ownership. [3]
*  very secure.

weakness:

*  Exist some drawbacks on closing mechanism. The use of memory locks improves efficiency but meanwhile increase the standards for system optimization. If the user’s optimization on the database and applications is not enough, then DB2 may have lock wait. [4]
*  Still imperfect on API and function support. [4]

reference:

*  http://www.ehow.com/info_12106599_advantages-db2.html
*  http://www-03.ibm.com/systems/power/software/i/db2/benefits.html
*  https://groups.google.com/forum/#!topic/comp.databases.ibm-db2/TufOncD8qO8
*  http://database.51cto.com/art/201103/251209.htm
  
##  33. Apache Hive:

keywords: relational, facebook, yahoo, amazon

strength:

*  “Fits low level interface requirement of Hadoop perfectly.” [1]
*  Can process data without actually storing them in the file system by the support of external tables. [1]
*  Supports table level data partitioning. [1]
*  Metadata store is available to make lookup easier. [1]
*  Great developer productivity. [2]
*  Can connect Hive queries to several Hadoop packages for statistical processing, including Apache Mahout, RHipe, RHive. [2]
*  Can explicitly control the map and reduce transform stages. [2]
*  Support rich data type. [3]
*  Partitioning and bucket: “partitioning helps split data into different chunks based on input value range, which allows to skip unwanted data while executing queries. Bucket split data is based on a hash function. Both help to improve the performance of querying.” [3]
*  Support queries with SQL-like operators. Can also redirect query output to a new table. [3]

weakness:

*  Does not support for update and deletion. [1]
*  Does not support singleton inserts. Data have to be loaded from file with LOAD command. [1]
*  No access control implementation. [1]
*  Does not support correlated sub queries. [1]
*  The batch nature of Map Reduce makes Hive perform bad when low-latency execution is needed for simple queries. [2]
*  Query compiler and optimizer are still young and need further development. [2]

reference:

*  http://www.gise.cse.iitb.ac.in/wiki/images/2/26/Hive.pdf
*  http://www.quora.com/What-are-the-advantages-of-Hive-over-SQL
*  http://www.learncomputer.com/hadoop-with-hive/

## 34. Memcached:

keywords: key-value, youtube, facebook, twitter

strength:

*  Memcached can compensate for insufficient ACID properties and never blocks. So if a thread invoking an I/O function, it don’t have to wait on any previous operation before executing. [1]
*  Cross Platform: applications on different platform can be used on other platform with complete transparency. [1]
*  Cross DBMS: can integrated into various of applications. [1]
*  Cheap: it’s free and open-source. [1]

weakness:

*  Size requirement: performs better on larger database and heavy reads writes loads. If application is a single server, then Memcached is not suitable for it. [1]
*  Documentation: there isn’t a good documentation support partly due to open-source. [1]
*  Volatility: if a memcached server crashes, then any data stored within the session also gone. [1]
*  Security: no authentication. [1]

reference:

*  http://xecanson.jp/memcached/memcached_BestDoc_English.pdf
*  https://ezeelive.wordpress.com/2011/07/25/memcache-caching-system-and-its-advantages/
  
##  35. MariaDB:

strength:

*  similar to MySQL so for MySQL users it’s very easy to start. [1]
*  The optimizer has been greatly improved so that the database has better performance for handling big data with subqueries. User also have additional control over how the optimizer makes decisions. [1,2]
*  Replication is faster if you have lots of concurrent updates. [2]
*  Provides better instrumentation through data dictionary information schema. [1]
*  Provide a command-line progress indicator so that no need to wait while executing time consuming alter table. [1]
*  Removes mutexes which perform badly.
*  Great improvements on row-based replication. SQL statements are being binary logged for row-based replication which is great for troubleshooting. [1]
*  compatible well. [4]
*  Open-source. [4]
*  more storage engines. [4]

weakness:

*  “Currently replication works only with the InnoDB storage engine. Any writes to table of other types, including system tables are not replicated.” [5]
*  “Unsupported explicit locking includes LOCK TABLES, FLUSH TABLES, etc.” [5]

reference:

*  http://www.infoworld.com/article/2611812/mysql/mysql-face-off--mysql-or-mariadb-.html
*  http://widwebway.com/en/blog?p=23
*  http://news.dice.com/2013/05/22/mariadb-vs-mysql-a-comparison-2/
*  http://markvaneijk.com/why-you-should-use-mariadb-instead-of-mysql
*  https://mariadb.com/kb/en/mariadb/mariadb-galera-cluster-known-limitations/
*  *  

