#IExtensionManager
  This class handles registration, lookup, and disposal of extensions. There should only be one of these per application instance. 

---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;Add(Dynamo.Extensions.IExtension)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Add an extension to the current application session. 

|*void* **&nbsp;&nbsp;Remove(Dynamo.Extensions.IExtension)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Remove an extension from the current application session. 


##Properties  
|*IEnumerable<*[IExtension](http://dynamods.github.io/DynamoAPI/Dynamo_Extensions/IExtension)*>* **&nbsp;&nbsp;Extensions {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The collection of currently registered extensions 




##Events  
|** **&nbsp;&nbsp;ExtensionAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event raised when an extension is added 


|** **&nbsp;&nbsp;ExtensionRemoved** |  stability index:1  
| ------------- | :--------------- 
|  Event raised when an extension is removed 



