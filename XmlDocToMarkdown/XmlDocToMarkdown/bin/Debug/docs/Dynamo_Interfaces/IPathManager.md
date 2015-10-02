#IPathManager
---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;AddResolutionPath(*String* path)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Call this method to add additional path for consideration when path resolution take place. 
| **path**
|The full path to be considered when PathManager attempt to resolve a file path. If this argument does not represent a valid directory path, this method throws an exception.




##Properties  
|*String* **&nbsp;&nbsp;DynamoCoreDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The directory in which DynamoCore.dll is guaranteed to be found. 


|*String* **&nbsp;&nbsp;UserDataDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The local directory that contains user specific data files. 


|*String* **&nbsp;&nbsp;CommonDataDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The local directory that contains common data files among users. 


|*String* **&nbsp;&nbsp;DefaultUserDefinitions {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The default directory that contains custom nodes created by the user. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;DefinitionDirectories {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Directories from where custom nodes are to be loaded. The implementor of this interface method should always guarantee that a non-empty list is returned, and that the first entry represents the default custom node directory. Custom nodes created are stored in the default directory, which is specific to the current user. Changes to custom nodes may or may not be saved to their current location depeding on write access. 


|*String* **&nbsp;&nbsp;CommonDefinitions {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The local directory that contains custom nodes created by all users. 


|*String* **&nbsp;&nbsp;LogDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The local directory where log files are generated. This directory is specific to the current user. 


|*String* **&nbsp;&nbsp;DefaultPackagesDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The default directory for saving packages downloaded through the package manager. This directory is specific to the current user. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;PackagesDirectories {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Directories from where packages are to be loaded. The implementor of this interface method should always guarantee that a non-empty list is returned, and that the first entry represents the default package directory. Packages downloaded through package manager are stored in the default package directory, which is specific to the current user. 


|*String* **&nbsp;&nbsp;ExtensionsDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The directory, which contains ExtensionDefinition .xml files 


|*String* **&nbsp;&nbsp;ViewExtensionsDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The directory, which contains ViewExtensionDefinition.xml files 


|*String* **&nbsp;&nbsp;SamplesDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The root directory where all sample files are stored. This directory is common to all users on the machine. 


|*String* **&nbsp;&nbsp;BackupDirectory {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The directory where the automatically saved files will be stored. 


|*String* **&nbsp;&nbsp;PreferenceFilePath {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Full path to the preference xml file. This setting file is specific to the current user. 


|*String* **&nbsp;&nbsp;GalleryFilePath {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Full path to the GalleryContent xml file. The file is located in the AppData/Dynamo/version/locale/ 


|*IEnumerable<*String*>* **&nbsp;&nbsp;NodeDirectories {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Folders in which node assemblies can be located. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;PreloadedLibraries {get;}** |  stability index:1  
| ------------- | :--------------- 
|  A list of node assembly names to be preloaded with Dynamo. 


|*Int32* **&nbsp;&nbsp;MajorFileVersion {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Major version of assembly file 


|*Int32* **&nbsp;&nbsp;MinorFileVersion {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Minor version of assembly file 



##Events  
####No public events defined

