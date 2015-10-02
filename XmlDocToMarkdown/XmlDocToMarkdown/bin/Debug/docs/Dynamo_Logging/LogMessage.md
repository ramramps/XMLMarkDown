#LogMessage
  Factory methods for creating log messages. 

---
##Constructors 
####No public constructors defined

##Methods  
|*[ILogMessage](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogMessage)* **&nbsp;&nbsp;Warning(*String* message,*[WarningLevel](http://dynamods.github.io/DynamoAPI/Dynamo/WarningLevel)* severity)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates a LogMessage representing a warning. 
| **message**
|
| **severity**
|

|*[ILogMessage](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogMessage)* **&nbsp;&nbsp;Error(*String* message)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates a LogMessage representing an error. 
| **message**
|

|*[ILogMessage](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogMessage)* **&nbsp;&nbsp;Error(*Exception* exception)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates a LogMessage representing an error. 
| **exception**
|

|*[ILogMessage](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogMessage)* **&nbsp;&nbsp;Info(*String* message)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Creates a basic LogMessage. 
| **message**
|

|*void* **&nbsp;&nbsp;Log(*[ILogger](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogger)* logger,*[ILogMessage](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/ILogMessage)* message)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Logs a LogMessage. 
| **logger**
|
| **message**
|






##Properties  
####No public properties defined

##Events  
####No public events defined

