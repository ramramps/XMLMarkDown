#CustomNodeManager
  Manages instantiation of custom nodes. All custom nodes known to Dynamo should be stored with this type. This object implements late initialization of custom nodes by providing a single interface to initialize custom nodes. 

---
##Constructors 


##Methods  
|*[CustomNodeWorkspaceModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/CustomNodeWorkspaceModel)* **&nbsp;&nbsp;GetWorkspaceById(*Guid* customNodeId)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Custom node workspace by a specified ID
|  Gets custom node workspace by a specified custom node ID 
| **customNodeId**
|Custom node ID of a requested workspace

|*[Function](http://dynamods.github.io/DynamoAPI/Dynamo_Nodes/Function)* **&nbsp;&nbsp;CreateCustomNodeInstance(*Guid* id,*String* nickname,*Boolean* isTestMode)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates a new Custom Node Instance. 
| **id**
|Identifier referring to a custom node definition.
| **nickname**
| Nickname for the custom node to be instantiated, used for error recovery if the given id could not be found. 
| **isTestMode**
| Flag specifying whether or not this should operate in "test mode". 

|*Guid* **&nbsp;&nbsp;GuidFromPath(*String* path)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Get a function id from a guid assuming that the file is already loaded. 
| **path**
|


|*void* **&nbsp;&nbsp;Remove(*Guid* guid)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Attempts to remove all traces of a particular custom node from Dynamo, assuming the node is not in a loaded workspace. 
| **guid**
|Custom node identifier.

|*Boolean* **&nbsp;&nbsp;Uninitialize(*Guid* guid)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Uninitialized a custom node. The information for the node is still retained, but the next time the node is queried for it's workspace / definition / an instace it will be re-initialized from disk. 
| **guid**
|Custom node identifier.

|*IEnumerable<*[CustomNodeInfo](http://dynamods.github.io/DynamoAPI/Dynamo/CustomNodeInfo)*>* **&nbsp;&nbsp;AddUninitializedCustomNodesInPath(*String* path,*Boolean* isTestMode,*Boolean* isPackageMember)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Scans the given path for custom node files, retaining their information in the manager for later potential initialization. 
| **path**
|Path on disk to scan for custom nodes.
| **isTestMode**
| Flag specifying whether or not this should operate in "test mode". 
| **isPackageMember**
| Indicates whether custom node comes from package or not. 




|*Boolean* **&nbsp;&nbsp;Contains(*Guid* guid)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Tells whether the custom node's unique identifier is inside of the manager (initialized or not) 
| **guid**
|The FunctionId

|*Boolean* **&nbsp;&nbsp;Contains(*String* name)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Tells whether the custom node's name is inside of the manager (initialized or not) 
| **name**
|The name of the custom node.

|*Boolean* **&nbsp;&nbsp;IsInitialized(*String* name)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** The name of the 
|  Tells whether the custom node is initialized in the manager 
| **name**
|The name of the node

|*Boolean* **&nbsp;&nbsp;IsInitialized(*Guid* guid)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Tells whether the custom node is initialized in the manager 
| **guid**
|Whether the definition is stored with the manager.












##Properties  
|*IEnumerable<*[CustomNodeDefinition](http://dynamods.github.io/DynamoAPI/Dynamo/CustomNodeDefinition)*>* **&nbsp;&nbsp;LoadedDefinitions {get;}** |  stability index:1  
| ------------- | :--------------- 
|  CustomNodeDefinitions for all loaded custom nodes, in load order. 


|*IEnumerable<*[CustomNodeWorkspaceModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/CustomNodeWorkspaceModel)*>* **&nbsp;&nbsp;LoadedWorkspaces {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All loaded custom node workspaces. 



##Events  
|** **&nbsp;&nbsp;DefinitionUpdated** |  stability index:1  
| ------------- | :--------------- 
|  An event that is fired when a definition is updated 


|** **&nbsp;&nbsp;InfoUpdated** |  stability index:1  
| ------------- | :--------------- 
|  An event that is fired when new or updated info is available for a custom node. 


|** **&nbsp;&nbsp;CustomNodeRemoved** |  stability index:1  
| ------------- | :--------------- 
|  An event that is fired when a custom node is removed from Dynamo. 




