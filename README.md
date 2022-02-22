# cloud-run-grpc-helloworld

build server image 
docker build -t gcr.io/teja-gaming-oss-dev/cloud-run-grpc-server -f Dockerfile.server .
docker push gcr.io/teja-gaming-oss-dev/cloud-run-grpc-server

run client
go run ./client/main.go

build client image 
docker build -t gcr.io/teja-gaming-oss-dev/cloud-run-grpc-client -f Dockerfile.client .
docker push gcr.io/teja-gaming-oss-dev/cloud-run-grpc-client

