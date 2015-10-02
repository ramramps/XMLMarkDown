#WorkspaceModel
---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;RemoveNode(*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)* model)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Removes a node from this workspace. This method does not raise a NodesModified event. (LC notes this is clearly not true) 
| **model**
|







|*Boolean* **&nbsp;&nbsp;Save(ProtoCore.RuntimeCore)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Save assuming that the Filepath attribute is set. 











|*void* **&nbsp;&nbsp;Dispose( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. 

|*void* **&nbsp;&nbsp;Clear( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Clears this workspace of nodes, notes, and connectors. 

|*Boolean* **&nbsp;&nbsp;SaveAs(*String* newPath,*RuntimeCore* core,*Boolean* isBackup)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Save to a specific file path, if the path is null or empty, does nothing. If successful, the CurrentWorkspace.FilePath field is updated as a side effect 
| **newPath**
|The path to save to
| **core**
|
| **isBackup**
|Indicates whether saved workspace is backup or not. If it's not backup, we should add it to recent files. Otherwise leave it.

|*void* **&nbsp;&nbsp;AddAndRegisterNode(Dynamo.Models.NodeModel)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Adds a node to this workspace. 






##Properties  
|*IEnumerable<*[PresetModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PresetModel)*>* **&nbsp;&nbsp;Presets {get;}** |  stability index:1  
| ------------- | :--------------- 
|  A set of input parameter states, this can be used to set the graph to a serialized state. 


|*DateTime* **&nbsp;&nbsp;LastSaved {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The date of the last save. 


|*String* **&nbsp;&nbsp;Author {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  An author of the workspace 


|*String* **&nbsp;&nbsp;Description {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A description of the workspace 


|*Boolean* **&nbsp;&nbsp;HasUnsavedChanges {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Are there unsaved changes in the workspace? 


|*IEnumerable<*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)*>* **&nbsp;&nbsp;Nodes {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All of the nodes currently in the workspace. 


|*IEnumerable<*[ConnectorModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/ConnectorModel)*>* **&nbsp;&nbsp;Connectors {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All of the connectors currently in the workspace. 


|*IEnumerable<*[NoteModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NoteModel)*>* **&nbsp;&nbsp;Notes {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All of the notes currently in the workspace. 



|*String* **&nbsp;&nbsp;FileName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Path to the file this workspace is associated with. If null or empty, this workspace has never been saved. 


|*String* **&nbsp;&nbsp;Name {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The name of this workspace. 


|*Double* **&nbsp;&nbsp;X {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Get or set the X position of the workspace. 


|*Double* **&nbsp;&nbsp;Y {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Get or set the Y position of the workspace 



|*Double* **&nbsp;&nbsp;Height {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Get the height of the workspace's bounds. 


|*Double* **&nbsp;&nbsp;Width {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Get the width of the workspace's bounds. 


|*[Rect2D](http://dynamods.github.io/DynamoAPI/Dynamo_Utilities/Rect2D)* **&nbsp;&nbsp;Rect {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Get the bounds of the workspace. 


|*Boolean* **&nbsp;&nbsp;CanUndo {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Determine if undo operation is currently possible. 


|*Boolean* **&nbsp;&nbsp;CanRedo {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Determine if redo operation is currently possible. 





|*Guid* **&nbsp;&nbsp;Guid {get;}** |  stability index:1  
| ------------- | :--------------- 
|  A unique identifier for the workspace. 



##Events  
|** **&nbsp;&nbsp;RequestNodeCentered** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a workspace requests that a Node or Note model is centered. 


|** **&nbsp;&nbsp;ZoomChanged** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired every time the zoom factor of a workspace changes. 


|** **&nbsp;&nbsp;CurrentOffsetChanged** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired every time the position offset of a workspace changes. 


|** **&nbsp;&nbsp;WorkspaceSaved** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when the workspace is saved. 


|** **&nbsp;&nbsp;NodeAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a node is added to the workspace. 


|** **&nbsp;&nbsp;NodeRemoved** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a node is removed from the workspace. 


|** **&nbsp;&nbsp;NodesCleared** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when nodes are cleared from the workspace. 


|** **&nbsp;&nbsp;NoteAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a note is added to the workspace. 


|** **&nbsp;&nbsp;NoteRemoved** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a note is removed from the workspace. 


|** **&nbsp;&nbsp;NotesCleared** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when notes are cleared from the workspace. 


|** **&nbsp;&nbsp;AnnotationAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when an annotation is added to the workspace. 


|** **&nbsp;&nbsp;AnnotationRemoved** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when an annotation is removed from the workspace. 


|** **&nbsp;&nbsp;AnnotationsCleared** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when annotations are cleared from the workspace. 


|** **&nbsp;&nbsp;ConnectorAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a connector is added to the workspace. 


|** **&nbsp;&nbsp;ConnectorDeleted** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when a connector is deleted from a workspace. 


|** **&nbsp;&nbsp;Disposed** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired when this workspace is disposed of. 


|** **&nbsp;&nbsp;Saving** |  stability index:1  
| ------------- | :--------------- 
|  Event that is fired during the saving of the workspace. Add additional XmlNode objects to the XmlDocument provided, in order to save data to the file. 





