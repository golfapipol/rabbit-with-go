# Demo Rabbitmq with Go

## How to develop

### Start rabbitmq

```bash
docker-compose up -d
```

### Run Consumer

```bash
go run cmd/consumer/main.go
```

### Run Producer

```bash
go run cmd/producer/main.go
```