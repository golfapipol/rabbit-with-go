# Demo Rabbitmq with Go

## How to develop

### Simple Run

#### Start rabbitmq

```bash
docker-compose up -d
```

#### Run Consumer

```bash
go run cmd/consumer/main.go
```

#### Run Producer

```bash
go run cmd/producer/main.go
```

### Run with Topic

#### Run Topic Consumer

```bash
go run cmd/topic/consumer/main.go "#"
```

#### Run Topic Producer

```bash
go run cmd/topic/producer/main.go "topic"
```