#AuthenticationManager
---
##Constructors 


##Methods  
|*void* **&nbsp;&nbsp;ToggleLoginState(System.Object)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Toggle current login state 

|*Boolean* **&nbsp;&nbsp;CanToggleLoginState(System.Object)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** none
|  Check if able to toggle login state 






##Properties  
|*Boolean* **&nbsp;&nbsp;HasAuthProvider {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Determines if the this.client has login capabilities 


|*LoginState* **&nbsp;&nbsp;LoginState {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Specifies whether the user is logged in or not. 


|*String* **&nbsp;&nbsp;Username {get;}** |  stability index:1  
| ------------- | :--------------- 
|  The username of the current user, if logged in. Otherwise null 


|*IAuthProvider* **&nbsp;&nbsp;AuthProvider {get;}** |  stability index:1  
| ------------- | :--------------- 
|  Current IAuthProvider 



##Events  


