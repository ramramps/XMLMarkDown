#CustomNodeDefinition
  Compiler definition of a Custom Node. 

---
##Constructors 


##Methods  






##Properties  
|*Boolean* **&nbsp;&nbsp;IsProxy {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Is this CustomNodeDefinition properly loaded? 


|*String* **&nbsp;&nbsp;FunctionName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Function name. 


|*Guid* **&nbsp;&nbsp;FunctionId {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function unique ID. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;DisplayParameters {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  User-friendly parameters 


|*IEnumerable<*[TypedParameter](http://dynamods.github.io/DynamoAPI/Dynamo_Library/TypedParameter)*>* **&nbsp;&nbsp;Parameters {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function parameters. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;ReturnKeys {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  If the function returns a dictionary, this specifies all keys in that dictionary. 


|*IEnumerable<*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)*>* **&nbsp;&nbsp;FunctionBody {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  NodeModels making up the body of the custom node. 


|*IEnumerable<*AssociativeNode*>* **&nbsp;&nbsp;OutputNodes {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Identifiers associated with the outputs of the custom node. 


|*String* **&nbsp;&nbsp;DisplayName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  User friendly name on UI. 


|*Type* **&nbsp;&nbsp;ReturnType {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Return type. 




|*String* **&nbsp;&nbsp;MangledName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Name to create custom node 



##Events  
####No public events defined

