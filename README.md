# CacheManager
CacheManager is made to help us manage/get data from our caches, e.g appfabric
I am desiging this application to be easy to use and extendable.
Whats my goal ? I need application that will get data from my AppFabricCache different cahces, check their stats every X configurable time, log the stats, save them to DB or whatever. 
So i am writing all the manager and data classes, and then implement a new assembly that inherits from CacheManager assembly, e.g AppFabricCacheManager. 

Each could write his own assembly for his own cache, and implement a different output, some will use MySQL, some will use MongoDB, they will all implement the IDataAdapter using their own concrete class. 
