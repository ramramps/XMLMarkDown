#UpdateValueParams
  This class encapsulates the input parameters that need to be passed into nodes when they are updated in the UI. 

---
##Constructors 
|*Type* **&nbsp;&nbsp;UpdateValueParams(*String* propertyName,*String* propertyValue,*ElementResolver* elementResolver)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
| 
| **propertyName**
|Name of the property whose value is to be updated. This parameter cannot be empty or null.
| **propertyValue**
|Value of the named property whose value is to be updated. This parameter can either be null or empty if the targeted property allows such values.This value comes directly from DynamoTextBox after user commits it. Overridden methods then use a specific IValueConverter to turn this string into another data type that it expects
| **elementResolver**
|responsible for resolving class namespaces


##Methods  





##Properties  




##Events  
####No public events defined

