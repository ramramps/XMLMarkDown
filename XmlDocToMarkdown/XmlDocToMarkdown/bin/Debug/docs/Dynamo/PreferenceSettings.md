#PreferenceSettings
  PreferenceSettings is a class for GUI to persist certain settings. Upon running of the GUI, those settings that are persistent will be loaded from a XML file from DYNAMO_SETTINGS_FILE. When GUI is closed, the settings into the XML file. 

---
##Constructors 


##Methods  
|*Boolean* **&nbsp;&nbsp;Save(*String* filePath)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Whether file is saved or error occurred.
|  Save PreferenceSettings in XML File Path if possible, else return false 
| **filePath**
|Path of the XML File

|*Boolean* **&nbsp;&nbsp;SaveInternal(*String* preferenceFilePath)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Whether file is saved or error occurred.
|  Save PreferenceSettings in a default directory when no path is specified. 
| **preferenceFilePath**
|The file path to save preference settings to. If this parameter is null or empty string, preference settings will be saved to the default path.

|*[PreferenceSettings](http://dynamods.github.io/DynamoAPI/Dynamo/PreferenceSettings)* **&nbsp;&nbsp;Load(*String* filePath)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:**  Stored PreferenceSettings from xml file or Default PreferenceSettings if xml file is not found. 
|  Return PreferenceSettings from XML path if possible, else return PreferenceSettings with default values 
| **filePath**
|Path of the XML File






##Properties  



|*Int32* **&nbsp;&nbsp;LibraryWidth {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The width of the library pane. 


|*Int32* **&nbsp;&nbsp;ConsoleHeight {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The height of the console display. 


|*Boolean* **&nbsp;&nbsp;ShowConnector {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Should connectors be visible? 


|*ConnectorType* **&nbsp;&nbsp;ConnectorType {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The types of connector: Bezier or Polyline. 


|*Boolean* **&nbsp;&nbsp;IsBackgroundPreviewActive {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Should the background 3D preview be shown? 


|*String* **&nbsp;&nbsp;NumberFormat {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The decimal precision used to display numbers. 


|*Int32* **&nbsp;&nbsp;MaxNumRecentFiles {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The maximum number of recent file paths to be saved. 


|*List<*String*>* **&nbsp;&nbsp;RecentFiles {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A list of recently opened file paths. 


|*List<*String*>* **&nbsp;&nbsp;BackupFiles {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A list of backup file paths. 


|*List<*String*>* **&nbsp;&nbsp;CustomPackageFolders {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A list of folders containing zero-touch nodes and custom nodes. 


|*List<*String*>* **&nbsp;&nbsp;PackageDirectoriesToUninstall {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  A list of packages used by the Package Manager to determine which packages are marked for deletion. 


|*Double* **&nbsp;&nbsp;WindowX {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The last X coordinate of the Dynamo window. 


|*Double* **&nbsp;&nbsp;WindowY {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The last Y coordinate of the Dynamo window. 


|*Double* **&nbsp;&nbsp;WindowW {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The last width of the Dynamo window. 


|*Double* **&nbsp;&nbsp;WindowH {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The last height of the Dynamo window. 


|*Boolean* **&nbsp;&nbsp;UseHardwareAcceleration {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Should Dynamo use hardware acceleration if it is supported? 


|*Int32* **&nbsp;&nbsp;BackupInterval {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  This defines how long (in milliseconds) will the graph be automatically saved. 


|*Int32* **&nbsp;&nbsp;BackupFilesCount {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  This defines how many files will be backed up. 


|*Boolean* **&nbsp;&nbsp;PackageDownloadTouAccepted {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Indicates if the user has accepted the terms of use for downloading packages from package manager. 


|*Boolean* **&nbsp;&nbsp;ShowEdges {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Indicates whether surface and solid edges will be rendered. 




##Events  


