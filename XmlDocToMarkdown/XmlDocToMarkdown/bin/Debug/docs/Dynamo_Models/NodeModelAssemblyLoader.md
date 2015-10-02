#NodeModelAssemblyLoader
  This class is responsible for loading types that derive from NodeModel. For information about package loading see the PackageLoader. For information about loading other libraries, see LibraryServices. 

---
##Constructors 


##Methods  

|*Boolean* **&nbsp;&nbsp;IsNodeSubType(System.Type)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** True if the type is node.
|  Determine if a Type is a node. Used by LoadNodesFromAssembly to figure out what nodes to load from other libraries (.dlls). 









##Properties  
|*IEnumerable<*Assembly*>* **&nbsp;&nbsp;LoadedAssemblies {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All assemblies that have been loaded into Dynamo. 



##Events  



