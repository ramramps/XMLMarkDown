#DynamoScheduler
---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;ScheduleForExecution(*[AsyncTask](http://dynamods.github.io/DynamoAPI/Dynamo_Core_Threading/AsyncTask)* asyncTask)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Callers of this method create an instance of AsyncTask derived class and call this method to schedule the task for execution. 
| **asyncTask**
|The task to execute asynchronously.

|*Boolean* **&nbsp;&nbsp;ProcessNextTask(*Boolean* waitIfTaskQueueIsEmpty)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** This method returns true if the task queue is not empty, or false otherwise. Note that this method returns false when scheduler begins to shutdown, even when the task queue is not empty.
|  An ISchedulerThread implementation calls this method so scheduler starts to process the next task in the queue, if there is any. Note that this method is meant to process only one task in queue. The implementation of ISchedulerThread is free to call this method again in a fashion that matches its task fetching behavior. 
| **waitIfTaskQueueIsEmpty**
|This parameter is only used if the task queue is empty at the time this method is invoked. When the task queue becomes empty, setting this to true will cause this call to block until either the next task becomes available, or when the scheduler is requested to shutdown.






##Properties  
|*[TimeStamp](http://dynamods.github.io/DynamoAPI/Dynamo_Core_Threading/TimeStamp)* **&nbsp;&nbsp;NextTimeStamp {get;}** |  stability index:1  
| ------------- | :--------------- 
|  AsyncTask base class calls this to obtain the new time-stamp value. 


|*Boolean* **&nbsp;&nbsp;IsTestMode {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Flag determining whether or not the scheduler is operating in Test Mode. 




##Events  
####No public events defined

