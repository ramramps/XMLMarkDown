#NodeFactory
  Manages factories and loaders for NodeModels. Can use registered factories and loaders to instantiate and load new NodeModels. 

---
##Constructors 


##Methods  




|*Boolean* **&nbsp;&nbsp;AddTypeFactoryAndLoader<*T*>( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Attempts to create a new factory and loader for a given type. 
| **TypeParam : *T* =** 

|*Boolean* **&nbsp;&nbsp;AddTypeFactoryAndLoader(*Type* nodeType)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Attempts to create a new factory and loader for a given type. 
| **nodeType**
|

|*void* **&nbsp;&nbsp;AddAlsoKnownAs(*Type* realType,*String* aka,*Boolean* overwrite)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Registers a type with another name that it may go by. 
| **realType**
|
| **aka**
|
| **overwrite**
|



|*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)* **&nbsp;&nbsp;CreateNodeFromXml(*XmlElement* elNode,*[SaveContext](http://dynamods.github.io/DynamoAPI/Dynamo_Models/SaveContext)* context)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates and Loads a new NodeModel from its Serialized form, using the node loaders registered in this factory. If loading fails, a Dummy Node is produced. 
| **elNode**
|
| **context**
|








##Properties  
####No public properties defined

##Events  


