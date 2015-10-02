#NodeSearchElement
  Base class for all Dynamo Node search elements. 

---
##Constructors 
####No public constructors defined

##Methods  
|*IEnumerable<*String*>* **&nbsp;&nbsp;SplitCategoryName(*String* categoryName)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** A list of output
|  Split a category name into individual category names splitting be DEFAULT_DELIMITER 
| **categoryName**
|The name

|*void* **&nbsp;&nbsp;ProduceNode( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Produces a new Node, via the ItemProduced event. 







##Properties  
|*Boolean* **&nbsp;&nbsp;IsVisibleInSearch {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Specified whether or not this entry should appear in search. 


|*String* **&nbsp;&nbsp;CreationName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The name that is used during node creation 


|*ICollection<*String*>* **&nbsp;&nbsp;Categories {get;}** |  stability index:1  
| ------------- | :--------------- 
|  List of nested categories this search element is contained in. 


|*String* **&nbsp;&nbsp;FullName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The full name of entry which consists of category name and entry name. 


|*String* **&nbsp;&nbsp;FullCategoryName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The category name of this node. 


|*String* **&nbsp;&nbsp;Name {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The name of this entry as it appears in the library. 


|*String* **&nbsp;&nbsp;Parameters {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The parameters of this entry, used for overloaded nodes. 


|*ICollection<*String*>* **&nbsp;&nbsp;SearchKeywords {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Collection of keywords which can be used to search for this element. 


|*String* **&nbsp;&nbsp;Description {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Description of the node. 



|*SearchElementGroup* **&nbsp;&nbsp;Group {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Group to which Node belongs to 


|*String* **&nbsp;&nbsp;Assembly {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Group to which Node belongs to 




|*ElementTypes* **&nbsp;&nbsp;ElementType {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Indicates whether it is custom node or zero-touch element. And whether this element comes from package or not. 



##Events  
|** **&nbsp;&nbsp;ItemProduced** |  stability index:1  
| ------------- | :--------------- 
|  Event fired when this search element produces a new NodeModel. This typically happens when it is selected in the library by the user. 



