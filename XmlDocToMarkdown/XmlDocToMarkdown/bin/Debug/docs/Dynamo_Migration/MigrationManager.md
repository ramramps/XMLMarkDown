#MigrationManager
---
##Constructors 


##Methods  
|*void* **&nbsp;&nbsp;AddMigrationType(*[TypeLoadData](http://dynamods.github.io/DynamoAPI/Dynamo_Models/TypeLoadData)* t)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Adds a new type containing Migration methods into this manager. 
| **t**
|

|*Boolean* **&nbsp;&nbsp;ProcessWorkspace(*[WorkspaceInfo](http://dynamods.github.io/DynamoAPI/Dynamo_Models/WorkspaceInfo)* workspaceInfo,*XmlDocument* xmlDoc)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Attempts to migrate a workspace to the current version of Dynamo. 
| **workspaceInfo**
|
| **xmlDoc**
|

|*void* **&nbsp;&nbsp;ProcessWorkspaceMigrations(*Version* currentVersion,*XmlDocument* xmlDoc,*Version* workspaceVersion)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Runs all migration methods found on the listed migration target types. 
| **currentVersion**
|
| **xmlDoc**
|
| **workspaceVersion**
|



|*XmlElement* **&nbsp;&nbsp;CreateFunctionNode(*XmlDocument* document,*XmlElement* assembly,*Int32* nickname,*String* signature)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the XmlElement that represents a DSFunction node with its basic function information with default attributes.
|  Call this method to create an empty DSFunction node that contains basic function node information. 
| **document**
|The XmlDocument to create the node in.
| **assembly**
|Name of the assembly that implements this function.
| **nickname**
|The nickname to display on the node.
| **signature**
|The signature of the function.




|*XmlElement* **&nbsp;&nbsp;CreateFunctionNodeFrom(*XmlElement* srcElement,*String[]* attribNames)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the resulting XmlElement with specified attributes duplicated from srcElement. The resulting XmlElement will also have a mandatory "type" attribute with value "Dynamo.Nodes.DSFunction". 
|  Call this method to create a XmlElement with a set of attributes carried over from the source XmlElement. The new XmlElement will have a name of "Dynamo.Nodes.DSFunction". 
| **srcElement**
|The source XmlElement object.
| **attribNames**
|The list of attribute names whose values are to be carried over to the resulting XmlElement. This list is mandatory and it cannot be empty. If a specified attribute cannot be found in srcElement, an empty attribute with the same name will be created in the resulting XmlElement.


|*XmlElement* **&nbsp;&nbsp;CreateFunctionNodeFrom(*XmlElement* srcElement)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the duplicated XmlElement with all attributes found in the source XmlElement. The resulting XmlElement will also have a mandatory "type" attribute with value "Dynamo.Nodes.DSFunction". 
|  Call this method to create a duplicated XmlElement with all the attributes found from the source XmlElement. 
| **srcElement**
|The source XmlElement to duplicate.


|*XmlElement* **&nbsp;&nbsp;CreateCodeBlockNodeFrom(*XmlElement* srcElement)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns an XmlElement that represents the resulting Code Block node.
|  Call this method to create an empty Code Block node, with all attributes carried over from an existing src XmlElement. 
| **srcElement**
|The source element from which the Code Block node XmlElement is constructed. All attributes of the source XmlElement will be copied over, and Code Block node specific attributes will be added.

|*XmlElement* **&nbsp;&nbsp;CloneAndChangeName(*XmlElement* element,*String* type,*String* nickname,*Boolean* cloneInnerXml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the cloned and updated XmlElement.
|  Call this method to create a clone of the original XmlElement and change its type at one go. This method preserves all the attributes while updating only the type name. 
| **element**
|The XmlElement to be cloned and the type name updated.
| **type**
|The fully qualified name of the new type.
| **nickname**
|The new nickname, by which this node is known.
| **cloneInnerXml**
|Parameter indicating whether the inner xml of the original node should be cloned.

|*XmlElement* **&nbsp;&nbsp;CreateDummyNode(*XmlElement* element,*Int32* inportCount,*Int32* outportCount)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns a new XmlElement representing the dummy node.
|  Call this method to create a dummy node, should a node failed to be migrated. This results in a dummy node with a description of what the original node type was, and also retain the number of input and output ports. 
| **element**
|XmlElement representing the original node which has failed migration.
| **inportCount**
|The number of input ports required on the new dummy node. This number must be a positive number greater or equal to zero.
| **outportCount**
|The number of output ports required on the new dummy node. This number must be a positive number greater or equal to zero.

|*XmlElement* **&nbsp;&nbsp;CreateMissingNode(*XmlElement* element,*Int32* inportCount,*Int32* outportCount)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns a new XmlElement representing the dummy node.
|  Call this method to create a dummy node, should a node failed to be migrated. This results in a dummy node with a description of what the original node type was, and also retain the number of input and output ports. 
| **element**
|XmlElement representing the original node which has failed migration.
| **inportCount**
|The number of input ports required on the new dummy node. This number must be a positive number greater or equal to zero.
| **outportCount**
|The number of output ports required on the new dummy node. This number must be a positive number greater or equal to zero.









##Properties  
|*List<*Type*>* **&nbsp;&nbsp;MigrationTargets {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A collection of types which contain migration methods. 



##Events  


