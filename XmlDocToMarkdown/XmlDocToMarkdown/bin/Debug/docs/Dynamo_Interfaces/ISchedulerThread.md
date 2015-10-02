#ISchedulerThread
---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;Initialize(*[IScheduler](http://dynamods.github.io/DynamoAPI/Dynamo_Core_Threading/IScheduler)* owningScheduler)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  DynamoScheduler calls this method to initialize and start this instance of scheduler thread. This call marks the point from which it is safe to call into DynamoScheduler. 
| **owningScheduler**
|A reference to the DynamoScheduler object which owns this instance of scheduler thread.

|*void* **&nbsp;&nbsp;Shutdown( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  DynamoScheduler calls this method to shutdown the scheduler thread. 


##Properties  
####No public properties defined

##Events  
####No public events defined

