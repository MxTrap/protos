protoc -I . --grpc-gateway_out ./gen/go \
--grpc-gateway_opt paths=source_relative \
proto/sso/sso.proto


protoc -I proto proto/sso/sso.proto --go_out=./gen/go/ \ 
--go_opt=paths=source_relative --go-grpc_out=./gen/go/ \ 
--go-grpc_opt=paths=source_relative
