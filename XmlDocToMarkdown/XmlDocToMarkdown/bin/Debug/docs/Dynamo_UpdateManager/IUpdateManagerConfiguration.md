#IUpdateManagerConfiguration
---
##Constructors 
####No public constructors defined

##Methods  

##Properties  
|*String* **&nbsp;&nbsp;DownloadSourcePath {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Defines download location for new installer 


|*String* **&nbsp;&nbsp;SignatureSourcePath {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Defines location for signature file to validate the new installer. 


|*Boolean* **&nbsp;&nbsp;CheckNewerDailyBuild {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Defines whether to consider daily builds for update, default is false. 


|*Boolean* **&nbsp;&nbsp;ForceUpdate {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Defines whether to force update, default vlaue is false. 


|*String* **&nbsp;&nbsp;InstallerNameBase {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Gets the base name of the installer to be used for upgrade. 


|*[IDynamoLookUp](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IDynamoLookUp)* **&nbsp;&nbsp;DynamoLookUp {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Gets IDynamoLookUp interface to search Dynamo installations on the system. 



##Events  
####No public events defined

