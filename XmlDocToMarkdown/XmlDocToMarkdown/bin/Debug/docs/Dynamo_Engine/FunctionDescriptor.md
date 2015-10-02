#FunctionDescriptor
  Describe a DesignScript function in a imported library 

---
##Constructors 


##Methods  





##Properties  

|*String* **&nbsp;&nbsp;Assembly {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Full path to the assembly the defined this function 


|*String* **&nbsp;&nbsp;ClassName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Class name of this function. If the functino is global function, return String.Empty. 


|*String* **&nbsp;&nbsp;FunctionName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function name. 


|*IEnumerable<*[TypedParameter](http://dynamods.github.io/DynamoAPI/Dynamo_Library/TypedParameter)*>* **&nbsp;&nbsp;Parameters {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function parameters. 


|*Type* **&nbsp;&nbsp;ReturnType {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function return type. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;ReturnKeys {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  If the function returns a dictionary, ReturnKeys is the key collection used in returned dictionary. 


|*Boolean* **&nbsp;&nbsp;IsVarArg {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Does the function accept a variable number of arguments? 





|*FunctionType* **&nbsp;&nbsp;Type {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Function type. 



|*String* **&nbsp;&nbsp;Description {get;}** |  stability index:1  
| ------------- | :--------------- 
|  A comment describing the function along with the signature 


|*IEnumerable<*Tuple<*String,String*>*>* **&nbsp;&nbsp;Returns {get;}** |  stability index:1  
| ------------- | :--------------- 
|  If the XML documentation for the function includes a returns field, this parameter contains a collection of tuples of output names to descriptions. Otherwise, this list will be empty. 


|*IEnumerable<*Tuple<*String,String*>*>* **&nbsp;&nbsp;InputParameters {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Inputs for Node 


|*String* **&nbsp;&nbsp;Category {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The category of this function. 


|*String* **&nbsp;&nbsp;QualifiedName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The string that is used to search for this function. 


|*String* **&nbsp;&nbsp;MangledName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  A unique name to identify a function. It is necessary when a function is overloaded. 


|*String* **&nbsp;&nbsp;Signature {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The full signature of the function. 


|*String* **&nbsp;&nbsp;UserFriendlyName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Return a user friendly name. E.g., for operator '+' it will return 'Add' 


|*String* **&nbsp;&nbsp;DisplayName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  QualifiedName with leading namespaces removed. 


|*Boolean* **&nbsp;&nbsp;IsVisibleInLibrary {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  This attribute sets, if this function is shown in library or not. 


|*Boolean* **&nbsp;&nbsp;CanUpdatePeriodically {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  This attribute sets whether the function enables periodic update of the workspace. 






##Events  
####No public events defined

