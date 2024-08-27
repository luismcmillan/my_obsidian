[[Interfaces]]
- When an interface doesn't contain any methods at all, it is called a "Marker" interface
- A marker interface is typically used by the JRE to determine that an object adheres to some rule or is able to perform an action, etc.
- not common for a developer to write their own marker interface.
- **common to use those that are included with the Java API**
```java
package java.io;
public interfce Serializable {
}
```
- a class that implements java.io.Serializable informs the JRE that objects of this type **may be serialized (a therm that means an object's state may be turned into a byte array which could be saved as a file, sent over a network, etc.)**