#NodeMigrationData
  This class contains the resulting nodes as a result of node migration. Note that this class may contain other information (e.g. connectors) in the future in the event a migration process results in other elements. 

---
##Constructors 


##Methods  
|*XmlElement* **&nbsp;&nbsp;FindConnector(*[PortId](http://dynamods.github.io/DynamoAPI/Dynamo_Migration/PortId)* startPort,*[PortId](http://dynamods.github.io/DynamoAPI/Dynamo_Migration/PortId)* endPort)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the notmatching connector if one is found, or null otherwise.
|  Call this method to find the connector in the associate XmlDocument, given its start and end port information. 
| **startPort**
|The identity of the start port.
| **endPort**
|The identity of the end port.

|*XmlElement* **&nbsp;&nbsp;FindFirstConnector(*[PortId](http://dynamods.github.io/DynamoAPI/Dynamo_Migration/PortId)* portId)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the first connector found to connect to the given port, or null otherwise.
|  Call this method to retrieve the first connector given a port. This method is a near equivalent of FindConnectors, but only return the first connector found. This way the caller codes can be simplified in a way that it does not have the validate the returned list for item count before accessing its element. 
| **portId**
|The identity of the port for which the first connector is to be retrieved.


|*IEnumerable<*XmlElement*>* **&nbsp;&nbsp;FindConnectors(*[PortId](http://dynamods.github.io/DynamoAPI/Dynamo_Migration/PortId)* portId)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the list of connectors connecting to the given port, or null if no connection is found connecting to it.
|  Given a port, get all connectors that connect to it. 
| **portId**
|The identity of the port for which connectors are to be retrieved.

|*void* **&nbsp;&nbsp;ReconnectToPort(*XmlElement* connector,*[PortId](http://dynamods.github.io/DynamoAPI/Dynamo_Migration/PortId)* port)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Reconnect a given connector to another port identified by "port". 
| **connector**
|The connector to update. Note that this parameter can be null, in which case there won't be any movement performed. This simplifies the caller so that it does not have to do a null-check before every call to this method (connectors may not present).
| **port**
|The new port to connect to.










##Properties  



##Events  
####No public events defined

