#NotifyPropertyChangedInvocatorAttribute
  Indicates that the method is contained in a type that implements [[T:System.ComponentModel.INotifyPropertyChanged]] interface and this method is used to notify that some property value changed 
  The method should be non-static and conform to one of the supported signatures: 
 **Example:**  _C# code_

```c#
    public class Foo : INotifyPropertyChanged {
      public event PropertyChangedEventHandler PropertyChanged;
      [NotifyPropertyChangedInvocator]
      protected virtual void NotifyChanged(string propertyName) { ... }
   
      private string _name;
      public string Name {
        get { return _name; }
        set { _name = value; NotifyChanged("LastName"); /* Warning */ }
      }
    }
    
    Examples of generated notifications:
    NotifyChanged("Property")NotifyChanged(() => Property)NotifyChanged((VM x) => x.Property)SetProperty(ref myField, value, "Property")
```

---
##Constructors 



##Methods  







##Properties  



##Events  
####No public events defined

