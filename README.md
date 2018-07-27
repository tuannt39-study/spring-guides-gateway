# Building a Gateway

Building a Gateway

- IDE: Intellij
- https://spring.io/guides/gs/gateway/
- https://github.com/spring-guides/gs-gateway


-


    http://localhost:9999/get
    

    {
        "args": {},
        "headers": {
            "Accept": "*/*",
            "Accept-Encoding": "gzip, deflate",
            "Cache-Control": "no-cache",
            "Connection": "close",
            "Forwarded": "proto=http;host=\"localhost:9999\";for=\"0:0:0:0:0:0:0:1:49495\"",
            "Hello": "World",
            "Host": "httpbin.org",
            "Postman-Token": "9149c244-a12b-4c58-b6ec-f2c2d2650243",
            "User-Agent": "PostmanRuntime/7.1.1",
            "X-Forwarded-Host": "localhost:9999"
        },
        "origin": "0:0:0:0:0:0:0:1, 171.253.125.124",
        "url": "http://localhost:9999/get"
    }
    
	
- 


    http://localhost:9999/delay/3
    Headers: Host:www.hystrix.com

	
    HTTP/1.1 200 OK
    transfer-encoding: chunked
    Content-Type: text/plain;charset=UTF-8
    
	
    fallback
