protoc -I=. --go_out=plugins=grpc:. user.proto

protoc --go-grpc_out=. --go-grpc_opt=paths=source_relative user.proto
