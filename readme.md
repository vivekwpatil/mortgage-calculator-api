REST API with some tools to calculate Mortgage properties like monthly payments.

At moment only supports to calculate the monthly payments of Linear Mortgage offered by most banks in The Netherlands.


## Pre-requisites

- Go 1.13
- dep (for dependency management, see: https://github.com/golang/dep)
- httpie (optional for testing)
- Docker (optional)

## Run
```bash
dep ensure
go run mortgage-calculator-api.go
```

## Build & Run Native
```bash
go build mortgage-calculator-api.go
./mortgage-calculator-api
```

## Docker
```bash
docker build -t mortgage-calculator-api .
docker run --rm -p5000:5000 mortgage-calculator-api
```
