#CodeBlockNodeModel
---
##Constructors 




##Methods  

|*List<*String*>* **&nbsp;&nbsp;GetDefinedVariableNames( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** List containing all the names
|  Returns the names of all the variables defined in this code block. 

|*Int32* **&nbsp;&nbsp;GetInportIndex(*[CodeBlockNodeModel](http://dynamods.github.io/DynamoAPI/Dynamo_Nodes/CodeBlockNodeModel)* variableName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:**  Index of the required port in the InPorts collection 
|  Returns the index of the port corresponding to the variable name given 
| **variableName**
| Name of the variable corresponding to an input port 

|*Int32* **&nbsp;&nbsp;GetOutportIndex(*String* variableName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Returns the corresponding output port index for a given defined variable 
| **variableName**
|




|*Type* **&nbsp;&nbsp;GetTypeHintForOutput(*Int32* index)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Return possible type of the output at specified output port. 
| **index**
|








































##Properties  





|*IEnumerable<*String*>* **&nbsp;&nbsp;TempVariables {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Temporary variables that generated in code. 
















































##Events  









