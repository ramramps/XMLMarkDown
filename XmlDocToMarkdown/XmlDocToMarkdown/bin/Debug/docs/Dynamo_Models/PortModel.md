#PortModel
---
##Constructors 


##Methods  

|*void* **&nbsp;&nbsp;DestroyConnectors( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Deletes all connectors attached to this PortModel. 

















##Properties  








|*[Point2D](http://dynamods.github.io/DynamoAPI/Dynamo_Utilities/Point2D)* **&nbsp;&nbsp;Center {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Center is used by connected connectors to update their shape The "center" of a port is derived from the type of port and offsets from the node origin based on the port's index in the ports collection. 


|*Boolean* **&nbsp;&nbsp;UsingDefaultValue {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Controls whether this port is set to use it's default value (true) or yield a closure (false). 


|*Boolean* **&nbsp;&nbsp;DefaultValueEnabled {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Controls whether the Use Default Value option is available. 


|*[Thickness](http://dynamods.github.io/DynamoAPI/Dynamo_Utilities/Thickness)* **&nbsp;&nbsp;MarginThickness {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Controls the space between successive output ports 














##Events  
|** **&nbsp;&nbsp;PortConnected** |  stability index:1  
| ------------- | :--------------- 
|  Event triggered when a port is connected. 


|** **&nbsp;&nbsp;PortDisconnected** |  stability index:1  
| ------------- | :--------------- 
|  Event triggered when a port is disconnected. 







