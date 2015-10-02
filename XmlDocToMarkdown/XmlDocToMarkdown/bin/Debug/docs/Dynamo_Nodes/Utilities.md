#Utilities
---
##Constructors 
####No public constructors defined

##Methods  

|*String* **&nbsp;&nbsp;PreprocessTypeName(*String* fullyQualifiedName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** The processed fully qualified name. For an example, the name "Dynamo.Elements.UV" will be returned as "Dynamo.Nodes.Uv". 
| 
| **fullyQualifiedName**
|A fully qualified name. An example of this would be "Dynamo.Elements.dynNode".

|*String* **&nbsp;&nbsp;TypedParametersToString(*[FunctionDescriptor](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/FunctionDescriptor)* descriptor,*String* overridePrefix)** |  stability index:1  
| ------------- | :--------------- 
|  This method returns a name for the icon based on name of the node. 
| **descriptor**
|Function descriptor, that contains all info about node.
| **overridePrefix**
| overridePrefix is used as default value for generating node icon name. If overridePrefix is empty, it uses QualifiedName property. e.g. Autodesk.DesignScript.Geometry.CoordinateSystem.ByOrigin 


|*IEnumerable<*KeyValuePair<*Guid,List<*String*>*>*>* **&nbsp;&nbsp;LoadTraceDataFromXmlDocument(*XmlDocument* document)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns a dictionary of deserialized node-data-list pairs loaded from the given XmlDocument.
|  Call this method to load serialized node-data-list pairs (through a prior call to SaveTraceDataToXmlDocument) from a given XmlDocument. 
| **document**
|The XmlDocument from which serialized node- data-list pairs are to be deserialized.






##Properties  
####No public properties defined

##Events  
####No public events defined

