#IUndoRedoRecorderClient
  An instance of UndoRedoRecorder is owned by an "undo client" object. In the context of Dynamo, the undo client is "Workspace". The undo recorder calls into the owning undo client in an undo/redo operation, causing the client to delete, reload or create the corresponding model. To qualify as an undo client, a class must implement this interface. 

---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;DeleteModel(*XmlElement* modelData)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  UndoRedoRecorder calls this method to delete a model in the client. 
| **modelData**
|The data representing the model to be deleted. It is important that this element contains identifiable information so that the corresponding model can be located in the client for deletion. 

|*void* **&nbsp;&nbsp;ReloadModel(*XmlElement* modelData)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  UndoRedoRecorder calls this method to request the client to reload a given model by giving its data. 
| **modelData**
|The xml data from which the corresponding model can be reloaded from.

|*void* **&nbsp;&nbsp;CreateModel(*XmlElement* modelData)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  UndoRedoRecorder calls this method to request a model to be created. 
| **modelData**
|The xml data from which the corresponding model can be re-created from.

|*[ModelBase](http://dynamods.github.io/DynamoAPI/Dynamo_Models/ModelBase)* **&nbsp;&nbsp;GetModelForElement(*XmlElement* modelData)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the model that modelData corresponds to.
|  UndoRedoRecorder calls this method to retrieve the up-to-date instance of the model before any undo/redo operation modifies the model. The up-to-date information of the model is important so that an undo operation can be redone (repopulated with the up-to-date data before the undo operation happens). 
| **modelData**
|The xml data representing the model which UndoRedoRecorder requires for serialization purposes.


##Properties  
####No public properties defined

##Events  
####No public events defined

