#DynamoModel
  The core model of Dynamo. 

---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;AddHomeWorkspace( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Add a new HomeWorkspace and set as current 

|*void* **&nbsp;&nbsp;AddCustomNodeWorkspace(*[CustomNodeWorkspaceModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/CustomNodeWorkspaceModel)* workspace)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Add a new, visible Custom Node workspace to Dynamo 
| **workspace**
|

|*void* **&nbsp;&nbsp;RemoveWorkspace(*[WorkspaceModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/WorkspaceModel)* workspace)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Remove a workspace from the dynamo model. 
| **workspace**
|

|*Boolean* **&nbsp;&nbsp;OpenCustomNodeWorkspace(*Guid* guid)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Opens an existing custom node workspace. 
| **guid**
|

|*void* **&nbsp;&nbsp;AddNodeToCurrentWorkspace(*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)* node,*Boolean* centered)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Adds a node to the current workspace. 
| **node**
|
| **centered**
|

|*void* **&nbsp;&nbsp;Copy( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Copy selected ISelectable objects to the clipboard. 

|*void* **&nbsp;&nbsp;Paste( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Paste ISelectable objects from the clipboard to the workspace. 

|*void* **&nbsp;&nbsp;AddToSelection(*Object* parameters)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Add an ISelectable object to the selection. 
| **parameters**
|The object to add to the selection.

|*void* **&nbsp;&nbsp;ClearCurrentWorkspace( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Clear the workspace. Removes all nodes, notes, and connectors from the current workspace. 



|*void* **&nbsp;&nbsp;ShutDown(*Boolean* shutdownHost)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  External components call this method to shutdown DynamoModel. This method marks 'ShutdownRequested' property to 'true'. This method is used rather than a public virtual method to ensure that the value of ShutdownRequested is set to true. 
| **shutdownHost**
|Set this parameter to true to shutdown the host application.

|*[DynamoModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/DynamoModel)* **&nbsp;&nbsp;Start( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Start DynamoModel with all default configuration options 



|*void* **&nbsp;&nbsp;Dispose( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. 

|*void* **&nbsp;&nbsp;ResetEngine(*Boolean* markNodesAsDirty)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Call this method to reset the virtual machine, avoiding a race condition by using a thread join inside the vm executive. TODO(Luke): Push this into a resync call with the engine controller 
| **markNodesAsDirty**
|Set this parameter to true to force reset of the execution substrait. Note that setting this parameter to true will have a negative performance impact.

|*void* **&nbsp;&nbsp;ForceRun( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Forces an evaluation of the current workspace by resetting the DesignScript VM. 

|*void* **&nbsp;&nbsp;OpenFileFromPath(*String* xmlPath)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Opens a Dynamo workspace from a path to an Xml file on disk. 
| **xmlPath**
|


















##Properties  
|*Boolean* **&nbsp;&nbsp;IsTestMode {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Testing flag is used to defer calls to run in the idle thread with the assumption that the entire test will be wrapped in an idle thread call. 


|*Boolean* **&nbsp;&nbsp;IsCrashing {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Specifies whether or not Dynamo is in a crash-state. 


|*Boolean* **&nbsp;&nbsp;EnableMigrationLogging {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Setting this flag enables creation of an XML in following format that records node mapping information - which old node has been converted to which to new node(s) 


|*[EngineController](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/EngineController)* **&nbsp;&nbsp;EngineController {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  DesignScript VM EngineController, used for this instance of Dynamo. 


|*Boolean* **&nbsp;&nbsp;ShutdownRequested {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Flag specifying whether a shutdown of Dynamo was requested. 


|*String* **&nbsp;&nbsp;Version {get;}** |  stability index:1  
| ------------- | :--------------- 
|  This version of Dynamo. 


|*[IUpdateManager](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IUpdateManager)* **&nbsp;&nbsp;UpdateManager {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  UpdateManager to handle automatic upgrade to higher version. 


|*[IPathManager](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/IPathManager)* **&nbsp;&nbsp;PathManager {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The path manager that configures path information required for Dynamo to function properly. See IPathManager interface for more details. 


|*[IExtensionManager](http://dynamods.github.io/DynamoAPI/Dynamo_Extensions/IExtensionManager)* **&nbsp;&nbsp;ExtensionManager {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Manages all extensions for Dynamo 


|*[DynamoScheduler](http://dynamods.github.io/DynamoAPI/Dynamo_Core_Threading/DynamoScheduler)* **&nbsp;&nbsp;Scheduler {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The Dynamo Scheduler, handles scheduling of asynchronous tasks on different threads. 


|*[WorkspaceModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/WorkspaceModel)* **&nbsp;&nbsp;CurrentWorkspace {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The active workspace in Dynamo. 


|*ObservableCollection<*[ModelBase](http://dynamods.github.io/DynamoAPI/Dynamo_Models/ModelBase)*>* **&nbsp;&nbsp;ClipBoard {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The copy/paste clipboard. 


|*Boolean* **&nbsp;&nbsp;IsShowingConnectors {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Specifies whether connectors are displayed in Dynamo. 


|*ConnectorType* **&nbsp;&nbsp;ConnectorType {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Specifies how connectors are displayed in Dynamo. 



|*[ITraceReconciliationProcessor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/ITraceReconciliationProcessor)* **&nbsp;&nbsp;TraceReconciliationProcessor {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  An object which implements the ITraceReconciliationProcessor interface, and is used for handlling the results of a trace reconciliation. 




##Events  











|** **&nbsp;&nbsp;CleaningUp** |  stability index:1  
| ------------- | :--------------- 
|  An event triggered when the workspace is being cleaned. 



|** **&nbsp;&nbsp;WorkspaceHidden** |  stability index:1  
| ------------- | :--------------- 
|  Event called when a workspace is hidden 



|** **&nbsp;&nbsp;RequestNodeSelect** |  stability index:1  
| ------------- | :--------------- 
|  An event which requests that a node be selected 




|** **&nbsp;&nbsp;EvaluationCompleted** |  stability index:1  
| ------------- | :--------------- 
|  An event triggered when a single graph evaluation completes. 


|** **&nbsp;&nbsp;RefreshCompleted** |  stability index:1  
| ------------- | :--------------- 
|  An event triggered when all tasks in scheduler are completed. 



|** **&nbsp;&nbsp;WorkspaceOpening** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired during the opening of the workspace. Use the XmlDocument object provided to conduct additional workspace opening operations. 


|** **&nbsp;&nbsp;ShutdownStarted** |  stability index:1  
| ------------- | :--------------- 
|  This event is raised right before the shutdown of DynamoModel started. When this event is raised, the shutdown is guaranteed to take place (i.e. user has had a chance to save the work and decided to proceed with shutting down Dynamo). Handlers of this event can still safely access the DynamoModel, the WorkspaceModel (along with its contents), and the DynamoScheduler. 


|** **&nbsp;&nbsp;ShutdownCompleted** |  stability index:1  
| ------------- | :--------------- 
|  This event is raised after DynamoModel has been shut down. At this point the DynamoModel is no longer valid and access to it should be avoided. 



