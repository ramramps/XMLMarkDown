#VariableInputNodeController
---
##Constructors 
####No public constructors defined

##Methods  
|*Int32* **&nbsp;&nbsp;GetInputIndexFromModel( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Fetches the index number to use for the next port. 

|*void* **&nbsp;&nbsp;RemoveInputFromModel( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Removes an input from this node. Called when the '-' button is clicked. 

|*void* **&nbsp;&nbsp;AddInputToModel( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Adds an input to this node. Called when the '+' button is clicked. 

|*void* **&nbsp;&nbsp;SetNumInputs(*Int32* numInputs)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Set the number of inputs. 
| **numInputs**
|


|*void* **&nbsp;&nbsp;SerializeInputCount(*XmlElement* nodeElement,*Int32* amount)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Serializes the input count of a VariableInputNode to Xml. 
| **nodeElement**
|
| **amount**
|








##Properties  
####No public properties defined

##Events  
####No public events defined

