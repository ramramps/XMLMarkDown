#XmlDocumentationExtensions
  Provides extension methods for reading XML documentation from reflected members. 

---
##Constructors 
####No public constructors defined

##Methods  
|*String* **&nbsp;&nbsp;GetDescription(*[TypedParameter](http://dynamods.github.io/DynamoAPI/Dynamo_Library/TypedParameter)* parameter,*XmlReader* xml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** The contents of the documentation description for the parameter.
|  Get a description of a parameter from the its documentation xml, using the corresponding FunctionDescriptor. 
| **parameter**
|The TypedParameter object corresponding to the parameter.
| **xml**
|

|*String* **&nbsp;&nbsp;GetSummary(*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* member,*XmlReader* xml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** The contents of the documentation summary tag.
|  Get a summary of a method from its documentation xml, using the corresponding FunctionDescriptor object. 
| **member**
|The FunctionDescriptor object corresponding to the method.
| **xml**
|

|*IEnumerable<*String*>* **&nbsp;&nbsp;GetSearchTags(*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* member,*XmlReader* xml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** A collection of search tags.
|  Get a collection of search tags for a method from its documentation xml, using the corresponding FunctionDescriptor object. 
| **member**
|The FunctionDescriptor object corresponding to the method.
| **xml**
|

|*IEnumerable<*Double*>* **&nbsp;&nbsp;GetSearchTagWeights(*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* member,*XmlReader* xml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** A collection of search weights, or an empty collection if the search weights tag is emtpy.
|  Get a collection of search tag weights for a method from its documentation xml, using the corresponding FunctionDescriptor object. 
| **member**
|The FunctionDescriptor object corresponding to the method.
| **xml**
|

|*IEnumerable<*Tuple<*String,String*>*>* **&nbsp;&nbsp;GetReturns(*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* member,*XmlReader* xml)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** A collection of return descriptions from the documentation returns tag.
|  Get a collection of return descriptions for a method from its documentation xml, using the corresponding FunctionDescriptor object. 
| **member**
|The FunctionDescriptor object corresponding to the method.
| **xml**
|






##Properties  
####No public properties defined

##Events  
####No public events defined

