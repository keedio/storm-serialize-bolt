#storm-serialize-bolt
##Description

This projects defines two bolts: first one gets the json message ({message:"XXXX", extraData:{data1:"XXX",data2:""}}) and let the bolts pass the values in the message field for the complete message and the extraData field as a JSONObject. The second one compounds the complete json again and injects it to the next bolt.
This two bolts avoid serializing/deserializing in each bolt.

## Compilation
Use maven
````
mvn clean package
```


