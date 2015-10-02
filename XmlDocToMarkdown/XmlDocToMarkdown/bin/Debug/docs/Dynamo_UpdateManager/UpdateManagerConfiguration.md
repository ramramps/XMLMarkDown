#UpdateManagerConfiguration
  Defines Update Manager Configuration settings. 

---
##Constructors 
|*String* **&nbsp;&nbsp;UpdateManagerConfiguration( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Default constructor 


##Methods  
|*[UpdateManagerConfiguration](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/UpdateManagerConfiguration)* **&nbsp;&nbsp;Load(*String* filePath,*[IUpdateManager](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IUpdateManager)* updateManager)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** UpdateManagerConfiguration
|  Loads the configurations from given xml file. 
| **filePath**
|Xml file path that contains configuration details.
| **updateManager**
|

|*void* **&nbsp;&nbsp;Save(*String* filePath,*[IUpdateManager](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IUpdateManager)* updateManager)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Saves this configuration to a given file in xml format. 
| **filePath**
|File path to save this configuration.
| **updateManager**
|

|*[UpdateManagerConfiguration](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/UpdateManagerConfiguration)* **&nbsp;&nbsp;GetSettings(*[IDynamoLookUp](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IDynamoLookUp)* lookUp,*[IUpdateManager](http://dynamods.github.io/DynamoAPI/Dynamo_UpdateManager/IUpdateManager)* updateManager)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Utility method to get the settings 
| **lookUp**
|IDynamoLookUp instance
| **updateManager**
|







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


|*String* **&nbsp;&nbsp;ConfigFilePath {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Return file path for the overriding config file. 




##Events  
####No public events defined

