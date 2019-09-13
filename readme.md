go run main.go

docker build -t go-docker .

docker run -d -p 8080:8080 go-docker

docker container ls

curl http://localhost:8080?name=github.com/aferlim

docker container stop $(docker container -q ls)