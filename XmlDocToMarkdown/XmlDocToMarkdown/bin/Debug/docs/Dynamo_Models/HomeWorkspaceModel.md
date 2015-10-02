#HomeWorkspaceModel
---
##Constructors 



##Methods  




|*void* **&nbsp;&nbsp;Clear( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Clears this workspace of nodes, notes, and connectors. 

|*void* **&nbsp;&nbsp;StartPeriodicEvaluation( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Start periodic evaluation using the currently set RunPeriod 

|*void* **&nbsp;&nbsp;StopPeriodicEvaluation( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Stop the on-going periodic evaluation, if there is any. 

|*void* **&nbsp;&nbsp;ResetEngine(*[EngineController](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/EngineController)* controller,*Boolean* markNodesAsDirty)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Call this method to reset the virtual machine, avoiding a race condition by using a thread join inside the vm executive. TODO(Luke): Push this into a resync call with the engine controller 
| **controller**
|
| **markNodesAsDirty**
|Set this parameter to true to force reset of the execution substrait. Note that setting this parameter to true will have a negative performance impact.


|*void* **&nbsp;&nbsp;Run( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  This method is typically called from the main application thread (as a result of user actions such as button click or node UI changes) to schedule an update of the graph. This call may or may not represent an actual update. In the event that the user action does not result in actual graph update (e.g. moving of node on UI), the update task will not be scheduled for execution. 

|*void* **&nbsp;&nbsp;GetExecutingNodes(*Boolean* showRunPreview)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  This function gets the set of nodes that will get executed in the next run. This function will be called when the nodes are modified or when showrunpreview is set the executing nodes will be sent via SetNodeDeltaState event. 
| **showRunPreview**
|This parameter controls the delta state computation 

|*IList<*ISerializable*>* **&nbsp;&nbsp;GetOrphanedSerializablesAndClearHistoricalTraceData( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Returns a list of ISerializable items which exist in the preloaded trace data but do not exist in the current CallSite data. 


























##Properties  

|*Boolean* **&nbsp;&nbsp;IsTestMode {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Flag specifying if this workspace is operating in "test mode". 


|*Boolean* **&nbsp;&nbsp;HasRunWithoutCrash {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Indicates whether a run has completed successfully. This flag is critical to ensuring that crashing run-auto files are not left in run-auto upon reopening. 


|*Int64* **&nbsp;&nbsp;EvaluationCount {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Evaluation count is incremented whenever the graph is evaluated. It is set to zero when the graph is Cleared. 


























##Events  























