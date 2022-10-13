# Secure WebSocket Server  (Rust, Warp with Docker)

```
cargo build

openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.rsa -out cert.pem

docker build -t rs_wss .

docker run -p 9231:9231 -t rs_wss
```