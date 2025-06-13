# 💾 Redis Cheat Sheet

## 🔧 Basic Commands
```bash
SET key "value"
GET key
DEL key
EXPIRE key 60
```

## 🔢 Lists and Hashes
```bash
RPUSH mylist a b c
LRANGE mylist 0 -1
HSET user:1 name "Alice"
HGETALL user:1
```

## 🔍 CLI
```bash
redis-cli
MONITOR
FLUSHALL
```