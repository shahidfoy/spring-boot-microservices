install microservice:
	`mvn clean install`
	
build microservice:
    `mvn clean package`

run spring application:
	`mvn spring-boot:run`
	
run spring application jar on different port:
	`java -Dserver.port=8001 -jar target\{micro-service-0.0.0}.jar`


important demo links for spring boot microservices:

	services
	  - http://localhost:8000/currency-exchange/from/USD/to/INR
	  - http://localhost:8001/currency-exchange/from/USD/to/INR
	  - http://localhost:8100/currency-converter/from/USD/to/INR/quantity/1000
	zuul
	  - http://localhost:8765/currency-exchange-service/currency-exchange/from/EUR/to/INR
	  - http://localhost:8765/currency-conversion-service/currency-converter-feign/from/usd/to/inr/quantity/1000
	eureka
	  - http://localhost:8761