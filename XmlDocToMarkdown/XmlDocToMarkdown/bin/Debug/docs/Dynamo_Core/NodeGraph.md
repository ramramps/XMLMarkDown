#NodeGraph
---
##Constructors 
####No public constructors defined

##Methods  
|*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)* **&nbsp;&nbsp;LoadNodeFromXml(*XmlElement* elNode,*[SaveContext](http://dynamods.github.io/DynamoAPI/Dynamo_Models/SaveContext)* context,*[NodeFactory](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeFactory)* nodeFactory)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates and initializes a NodeModel from its Xml representation. 
| **elNode**
|XmlElement for a NodeModel.
| **context**
|The serialization context for initialization.
| **nodeFactory**
|A NodeFactory, to be used to create the node.


|*[NoteModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NoteModel)* **&nbsp;&nbsp;LoadNoteFromXml(*XmlNode* note)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates and initializes a NoteModel from its Xml representation. 
| **note**
|


|*[NodeGraph](http://dynamods.github.io/DynamoAPI/Dynamo_Core/NodeGraph)* **&nbsp;&nbsp;LoadGraphFromXml(*XmlDocument* xmlDoc,*[NodeFactory](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeFactory)* nodeFactory)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Loads NodeModels, ConnectorModels, and NoteModels from an XmlDocument. 
| **xmlDoc**
|An XmlDocument representing a serialized Dynamo workspace.
| **nodeFactory**
|A NodeFactory, used to load and instantiate nodes.
| **elementResolver**
|






##Properties  







##Events  
####No public events defined

