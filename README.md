# multi-wsdl-testing-api
Created for etsting multiple wsdl with logger stamping in cloudhub2.0


http://localhost:8081/api/HelloWorldService/HelloWorldPort?wsdl



mvn clean deploy -DmuleDeploy -Dserver=anypoint-connected-app -DappName=multi-wsdl-testing-api-dev -DmuleVersion=4.4.0 -DtargetName=Cloudhub-US-East-2 -Denvironment=Sandbox -Dreplicas=1 -DreplicasType=0.1 -Dbranch.name=dev -Ddecryption.key=goodluckDEV12345
