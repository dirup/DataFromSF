# DataFromSF
This service is responsible for connecting to SFDC and do a batch pull of object data and transform/write it 
into a csv/parquet and save it in local file system. This service can be triggered at T:00 hours on a daily basis.

This Microservice is developed using Springboot. Current project structure is the general template structure using Springboot.

The main component in this microservice is JavaSFController, this component connects to Salesforce and export the data to local file system.

All the configurable properties in this microservices like username, password, soapAuthEndPoint, bulkAuthEndPoint are maintained in application.properties under resources folder
file, so it is easy to configure them even in runtime and supports loose coupling.

Salesforce java jar is required to connect to Saalesforce using java code.

