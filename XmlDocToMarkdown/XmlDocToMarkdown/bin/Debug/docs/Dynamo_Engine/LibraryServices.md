#LibraryServices
  LibraryServices is a singleton class which manages builtin libraries as well as imported libraries. It is across different sessions. 

---
##Constructors 


##Methods  

|*void* **&nbsp;&nbsp;UpdateLibraryCoreData( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Copy properties from the liveCore The properties to copy are only those used by the library core 








|*IEnumerable<*[FunctionGroup](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionGroup)*>* **&nbsp;&nbsp;GetFunctionGroups(*String* library)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Get function groups from an imported library. 
| **library**
|Library path

|*IEnumerable<*[FunctionGroup](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionGroup)*>* **&nbsp;&nbsp;GetAllFunctionGroups( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Return all function groups. 

|*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* **&nbsp;&nbsp;GetFunctionDescriptor(*String* library,*String* mangledName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Get function descriptor from the managled function name. name. 
| **library**
|Library path
| **mangledName**
|Mangled function name

|*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* **&nbsp;&nbsp;GetFunctionDescriptor(*String* managledName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Get function descriptor from the managed function name. 
| **managledName**
|

|*Boolean* **&nbsp;&nbsp;IsLibraryLoaded(*String* library)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:**  true even if the same library name is loaded from different paths 
|  Checks if a given library is already loaded or not. Only unique assembly names are allowed to be loaded 
| **library**
| can be either the full path or the assembly name 

|*Boolean* **&nbsp;&nbsp;ImportLibrary(*String* library)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Import a library (if it hasn't been imported yet). 
| **library**
|







##Properties  

|*IEnumerable<*String*>* **&nbsp;&nbsp;ImportedLibraries {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Get a list of imported libraries. 


|*IEnumerable<*[FunctionGroup](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionGroup)*>* **&nbsp;&nbsp;BuiltinFunctionGroups {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Get builtin function groups. 
| **Return Value:** 


|*IEnumerable<*[FunctionGroup](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionGroup)*>* **&nbsp;&nbsp;ImportedFunctionGroups {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Get all imported function groups. 



##Events  





