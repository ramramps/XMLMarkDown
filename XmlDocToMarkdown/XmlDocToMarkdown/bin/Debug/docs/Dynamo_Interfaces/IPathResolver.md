#IPathResolver
---
##Constructors 
####No public constructors defined

##Methods  

##Properties  
|*IEnumerable<*String*>* **&nbsp;&nbsp;AdditionalResolutionPaths {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Additional directories that should be considered when path resolution is done for a library that does not contain full path information. The return value of this property should never be null. Each entry must represent a valid directory, otherwise DirectoryNotFoundException exception is thrown. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;AdditionalNodeDirectories {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Additional directories in which node assemblies can be located. The return value of this property should never be null. Each entry must represent a valid directory, otherwise DirectoryNotFoundException exception is thrown. 


|*IEnumerable<*String*>* **&nbsp;&nbsp;PreloadedLibraryPaths {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Libraries to be preloaded as part of Dynamo start up sequence. Each entry in this list can either represent full path to a library, or just the assembly name. If absolute path information is not supplied, the library will be looked up through both predefined and additional resolution paths. The return value of this property should never be null. 


|*String* **&nbsp;&nbsp;UserDataRootFolder {get;}** |  stability index:1  
| ------------- | :--------------- 
|  This property represents the root folder where user specific data files are stored. If this property returns a null or empty string, then PathManager falls back to using "%ProgramData%\Dynamo". If this property returns a string that does not represent an existing folder, PathManager will attempt to create a new directory. If the property does not represent a valid path string, an exception will be thrown by the underlying system IO API invoked. Note that this path should not include the version number as it will be appended by PathManager. 


|*String* **&nbsp;&nbsp;CommonDataRootFolder {get;}** |  stability index:1  
| ------------- | :--------------- 
|  This property represents the root folder where application common data files (i.e. shared among all users on the same machine) are stored. If this property returns a null or empty string, then PathManager falls back to using "%AppData%\Dynamo". If this property returns a string that does not represent an existing folder, PathManager will attempt to create a new directory. If the property does not represent a valid path string, an exception will be thrown by the underlying system IO API invoked. Note that this path should not include the version number as it will be appended by PathManager. 



##Events  
####No public events defined

