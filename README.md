### Get protoc installed. Follow google instructions.
### ... also brew works as well

## To Run Server
- `go run usermgmt_server/usermgmt_server.go`
- `enter`

## To Run Client
- `go run usermgmt_client/usermgmt_client.go`
- `enter` 

## What to expect
Server Terminal will dump out "Received: {user-information}" with a time stamp
Client Terminal will dump out "User Details: NAME {name} AGE {age} ID {id}"

This is a unary service, which means that the server is waiting for the inbound message to come from the client. 
It seems to be essentially the same thing as an SDK, or API request, or something of that nature.. 

There are (3) count em THREE other types of services that can be made with gRPC (Server Stream, Client Stream, and Bi-Stream). Someday I will learn those as well.