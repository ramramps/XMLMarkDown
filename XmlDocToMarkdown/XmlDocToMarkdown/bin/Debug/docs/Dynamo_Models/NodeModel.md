#NodeModel
---
##Constructors 
####No public constructors defined

##Methods  
|*void* **&nbsp;&nbsp;RegisterInputPorts( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Reads inputs list and adds ports for each input. 

|*void* **&nbsp;&nbsp;RegisterOutputPorts( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Reads outputs list and adds ports for each output 

|*void* **&nbsp;&nbsp;RegisterAllPorts( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Updates UI so that all ports reflect current state of InPortData and OutPortData. 

|*[PortModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortModel)* **&nbsp;&nbsp;AddPort(*[PortType](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortType)* portType,*[PortData](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortData)* data,*Int32* index)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Add a port to this node. If the port already exists, return that port. 
| **portType**
|
| **data**
|
| **index**
|

|*String* **&nbsp;&nbsp;PrintExpression( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** S-Expression
|  Creates a Scheme representation of this dynNode and all connected dynNodes. 




|*void* **&nbsp;&nbsp;RequestVisualUpdateAsync(*[IScheduler](http://dynamods.github.io/DynamoAPI/Dynamo_Core_Threading/IScheduler)* scheduler,*[EngineController](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/EngineController)* engine,*[IRenderPackageFactory](http://dynamods.github.io/DynamoAPI/Dynamo_Interfaces/IRenderPackageFactory)* factory,*Boolean* forceUpdate)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Call this method to asynchronously regenerate render package for this node. This method accesses core properties of a NodeModel and therefore is typically called on the main/UI thread. 
| **scheduler**
|An IScheduler on which the task will be scheduled.
| **engine**
|The EngineController which will be used to get MirrorData for the node.
| **factory**
|An IRenderPackageFactory which will be used to generate IRenderPackage objects.
| **forceUpdate**
|Normally, render packages are only generated when the node's IsUpdated parameter is true. By setting forceUpdate to true, the render packages will be updated.

|*void* **&nbsp;&nbsp;DispatchOnUIThread(*Action* a)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Called by nodes for behavior that they want to dispatch on the UI thread Triggers event to be received by the UI. If no UI exists, behavior will not be executed. 
| **a**
|

|*String* **&nbsp;&nbsp;GetDescriptionStringFromAttributes( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** The value or "No description provided"
|  Get the description from type information 

|*IdentifierNode* **&nbsp;&nbsp;GetAstIdentifierForOutputIndex(*Int32* outputIndex)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Identifier corresponding to the given output port.
|  Fetches the ProtoAST Identifier for a given output port. 
| **outputIndex**
|Index of the output port.

|*Type* **&nbsp;&nbsp;GetTypeHintForOutput(System.Int32)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  The possible type of output at specified port. This type information is not necessary to be accurate. 

|*MirrorData* **&nbsp;&nbsp;GetValue(*Int32* outPortIndex,*[EngineController](http://dynamods.github.io/DynamoAPI/Dynamo_Engine/EngineController)* engine)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Gets the most recent value of this node stored in an EngineController that has evaluated it. 
| **outPortIndex**
|
| **engine**
|

|*void* **&nbsp;&nbsp;SetNickNameFromAttribute( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Sets the nickname of this node from the attributes on the class definining it. 






|*Boolean* **&nbsp;&nbsp;HasInput(*Int32* data)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** True if there is an input, false otherwise.
|  Checks if there is an input for a certain port. 
| **data**
|Index of the port to look for an input for.

|*Boolean* **&nbsp;&nbsp;HasConnectedInput(*Int32* data)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** True if there is an input, false otherwise.
|  Checks if there is a connected input for a certain port. This does not count default values as an input. 
| **data**
|Index of the port to look for an input for.

|*Boolean* **&nbsp;&nbsp;HasOutput(*Int32* portData)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** True if there is an output, false otherwise.
|  Checks if there is an output for a certain port. 
| **portData**
|Index of the port to look for an output for.

|*void* **&nbsp;&nbsp;ClearRuntimeError( )** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Clears the errors/warnings that are generated when running the graph. If the node has a value supplied for the persistentWarning, then the node's State will be set to ElementState.Persistent and the ToolTipText will be set to the persistent warning. Otherwise, the State will be set to ElementState.Dead 




|*void* **&nbsp;&nbsp;Warning(*String* p,*Boolean* isPersistent)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Set a warning on a node. 
| **p**
|The warning text.
| **isPersistent**
|Is the warning persistent? If true, the warning will not be cleared when the node is next evaluated and any additional warning messages will be concatenated to the persistent error message. If false, the warning will be cleared on the next evaluation.

|*void* **&nbsp;&nbsp;NotifyAstBuildBroken(*String* p)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Change the state of node to ElementState.AstBuildBroken and display "p" in tooltip window. 
| **p**
|














##Properties  
|*String* **&nbsp;&nbsp;CreationName {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The unique name that was created the node by 


|*ObservableCollection<*[PortData](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortData)*>* **&nbsp;&nbsp;InPortData {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Definitions for the Input Ports of this NodeModel. 


|*ObservableCollection<*[PortData](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortData)*>* **&nbsp;&nbsp;OutPortData {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Definitions for the Output Ports of this NodeModel. 


|*IEnumerable<*[ConnectorModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/ConnectorModel)*>* **&nbsp;&nbsp;AllConnectors {get;}** |  stability index:1  
| ------------- | :--------------- 
|  All of the connectors entering and exiting the NodeModel. 


|*Boolean* **&nbsp;&nbsp;IsCustomFunction {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Returns whether this node represents a built-in or custom function. 


|*Boolean* **&nbsp;&nbsp;IsVisible {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Returns whether the node is to be included in visualizations. 


|*Boolean* **&nbsp;&nbsp;IsUpstreamVisible {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Returns whether the node aggregates its upstream connections for visualizations. 


|*Boolean* **&nbsp;&nbsp;IsInputNode {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Input nodes are used in Customizer and Presets. Input nodes can be numbers, number sliders, strings, bool, code blocks and custom nodes, which don't specify path. 


|*Boolean* **&nbsp;&nbsp;IsSelectedInput {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Specifies whether an input node should be included in a preset. By default, this field is set to true. 


|*ElementState* **&nbsp;&nbsp;State {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The Node's state, which determines the coloring of the Node in the canvas. 


|*Boolean* **&nbsp;&nbsp;IsInErrorState {get;}** |  stability index:1  
| ------------- | :--------------- 
|  If the state of node is Error or AstBuildBroken 


|*String* **&nbsp;&nbsp;ToolTipText {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Text that is displayed as this Node's tooltip. 


|*Boolean* **&nbsp;&nbsp;OverrideNameWithNickName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Should we override the displayed name with this Node's NickName property? 


|*String* **&nbsp;&nbsp;NickName {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  The name that is displayed in the UI for this NodeModel. 


|*ObservableCollection<*[PortModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortModel)*>* **&nbsp;&nbsp;InPorts {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Collection of PortModels representing all Input ports. 


|*ObservableCollection<*[PortModel](http://dynamods.github.io/DynamoAPI/Dynamo_Models/PortModel)*>* **&nbsp;&nbsp;OutPorts {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Collection of PortModels representing all Output ports. 




|*LacingStrategy* **&nbsp;&nbsp;ArgumentLacing {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Control how arguments lists of various sizes are laced. 


|*String* **&nbsp;&nbsp;Name {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Name property 


|*String* **&nbsp;&nbsp;Category {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Category property 



|*Boolean* **&nbsp;&nbsp;IsUpdated {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  If the node is updated in LiveRunner's execution 


|*List<*String*>* **&nbsp;&nbsp;Tags {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Search tags for this Node. 


|*String* **&nbsp;&nbsp;Description {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Description of this Node. 



|*IdentifierNode* **&nbsp;&nbsp;AstIdentifierForPreview {get;}** |  stability index:1  
| ------------- | :--------------- 
|  ProtoAST Identifier for result of the node before any output unpacking has taken place. If there is only one output for the node, this is equivalent to GetAstIdentifierForOutputIndex(0). 


|*Boolean* **&nbsp;&nbsp;IsConvertible {get;}** |  stability index:1  
| ------------- | :--------------- 
|  If this node is allowed to be converted to AST node in nodes to code conversion. 


|*String* **&nbsp;&nbsp;AstIdentifierBase {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Return a variable whose value will be displayed in preview window. Derived nodes may overwrite this function to display default value of this node. E.g., code block node may want to display the value of the left hand side variable of last statement. 


|*Boolean* **&nbsp;&nbsp;DisplayLabels {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Enable or disable label display. Default is false. 


|*Boolean* **&nbsp;&nbsp;IsPartiallyApplied {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Is this node being applied partially, resulting in a partial function? 


|*Boolean* **&nbsp;&nbsp;RaisesModificationEvents {get;set;}** |  stability index:1  
| ------------- | :--------------- 
|  Indicate if the node should respond to NodeModified event. It always should be true, unless is temporarily set to false to avoid flood of Modified event. 


|*Boolean* **&nbsp;&nbsp;IsTopMostNode {get;}** |  stability index:1  
| ------------- | :--------------- 
|  If node is connected to some other node(other than Output) then it is not a 'top' node 
















##Events  
|** **&nbsp;&nbsp;Modified** |  stability index:1  
| ------------- | :--------------- 
|  Event fired when the node's DesignScript AST should be recompiled 


|** **&nbsp;&nbsp;ConnectorAdded** |  stability index:1  
| ------------- | :--------------- 
|  Event fired when a new ConnectorModel has been attached to one of this node's inputs. 


|** **&nbsp;&nbsp;RequestRenderPackages** |  stability index:1  
| ------------- | :--------------- 
| 








