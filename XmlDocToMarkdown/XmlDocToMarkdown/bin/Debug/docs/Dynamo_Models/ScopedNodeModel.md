#ScopedNodeModel
  ScopedNodeModel will put its children in its scope so that they won't get compiled in global scope. 

---
##Constructors 


##Methods  
|*IEnumerable<*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)*>* **&nbsp;&nbsp;GetInScopeNodesForInport(*Int32* portIndex,*Boolean* checkEscape,*Boolean* isInclusive)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Get all nodes that in its input ports's scope. A node is in its scope if that node is one of its upstream nodes. 
| **portIndex**
|Inport index
| **checkEscape**
| If need to exclude nodes that one of their downstream nodes are not in the scope 
| **isInclusive**
| If a upstream node is ScopedNodeModel, need to include all upstream nodes of that node. 

|*IEnumerable<*[NodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/NodeModel)*>* **&nbsp;&nbsp;GetInScopeNodes(*Boolean* checkEscape,*Boolean* isInclusive)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Return all nodes that are in the scope of this node. nodes are not in the scope. 
| **checkEscape**
| Specifies if need to exclude nodes that one of their downstream nodes are not in the scope 
| **isInclusive**
| If one of its upstream node is ScopedNodeModel, if need to include all upstream nodes of that node. 













































##Properties  















































##Events  









