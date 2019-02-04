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

- # - หมายถึง รับหมดไม่ว่าจะส่งเป็น routing key ไหนเข้ามา

#### Run Topic Producer

```bash
go run cmd/topic/producer/main.go "routing-key"
```

- routing-key - ชื่อ routing-key ที่ exchange ใช้ในการส่งเข้า queue