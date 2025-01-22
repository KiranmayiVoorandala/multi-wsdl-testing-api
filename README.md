# multi-wsdl-testing-api
Created for etsting multiple wsdl with logger stamping in cloudhub2.0

########Local Endpoint:
http://localhost:8081/api/HelloWorldService/HelloWorldPort?wsdl

#####cloudhub 2.0 Endpoint 
https://multi-wsdl-testing-api-dev-lewuz5.5sc6y6-2.usa-e2.cloudhub.io/api/HelloWorldService/HelloWorldPort?wsdl
https://multi-wsdl-testing-api-dev-lewuz5.5sc6y6-2.usa-e2.cloudhub.io/api/CalculatorService/CalculatorPort?wsdl
https://multi-wsdl-testing-api-dev-lewuz5.5sc6y6-2.usa-e2.cloudhub.io/api/ContractSOAPQSService/ContractSOAPQSPort?wsdl
https://multi-wsdl-testing-api-dev-lewuz5.5sc6y6-2.usa-e2.cloudhub.io/api/NDPEventOAGSvc/NDPEventOAGSvcBindingPort?wsdl
	
############Maven Comand 
publish to an exchange : mvn clean deploy	
Deploy to runtime manager : mvn clean deploy -DmuleDeploy -Dserver=anypoint-connected-app -DappName=multi-wsdl-testing-api-dev -DmuleVersion=4.4.0 -DtargetName=Cloudhub-US-East-2 -Denvironment=Sandbox -Dreplicas=1 -DreplicasType=0.1 -Dbranch.name=dev -Ddecryption.key=goodluckDEV12345
