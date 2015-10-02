#AsyncTask
---
##Constructors 
####No public constructors defined

##Methods  





##Properties  
|*TaskPriority* **&nbsp;&nbsp;Priority {get;}** |  stability index:1  
| ------------- | :--------------- 
|  DynamoScheduler sorts tasks base on two key factors: the priority of a task, and the relative importance between two tasks that has the same priority. During task reprioritization process, DynamoScheduler first sorts the tasks in accordance to their AsyncTask.Priority property. The resulting ordered list is then sorted again by calling AsyncTask.Compare method to determine the relative importance among tasks having the same priority. 



##Events  
|** **&nbsp;&nbsp;Completed** |  stability index:1  
| ------------- | :--------------- 
|  This event is raised when the AsyncTask is completed. The event is being raised in the context of ISchedulerThread, any UI element access that is needed should be dispatched onto the UI dispatcher. 



