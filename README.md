
 Data base Lasrning  day -1




















Cache:- 
if the l million  request is hitting to data base is then data base will crash or preform will be decreases  so  here we user cache
-> so here we start spring boot application where first request is check whether data in cases or not if not then hit database and retrieve information then second request is come check whether data is present or not if present then I print that that present in cache
caching is use for improving the performance of the application 
two types of cache in java 
1) in-memory cache ->ConcurrentcHashMapCache, Caffeine Cache  -> we can create the cache inside the spring boot application  
 advantage of this cache is very strong is present inside our spring boot application

disadvantage is if out application is suddenly stop or rebutted then it can clear hole the data form cache it again connect wit the data base 
to avoid this we use Distributive cacahe

2)Distributive cache -> redis,hazelcast :- 

radis ->we need to installed it as a sperate service if we have three application then we need to create only one separate copy of cache it will run on seprate port 

advantage of this:- if application stop or reboot then cache maintain the data

it provider more features like 
1)clusting of cache _> here we can create the multiple duplicate copies if any one cluster the data is lost or server is stop then it still maintain in another cluster  if any cluster is updated then is also update in another cahche also because it sync

