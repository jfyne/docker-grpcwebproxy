# Dockerfile for github.com/improbable-eng/grpc-web

github.com/improbable-eng/grpc-web

## Usage
```bash
docker run --net="host" -v ${PWD}/certs:/certs --rm -it jfyne/docker-grpcwebproxy \
        /grpcwebproxy \
        --server_tls_cert_file=/certs/localhost.crt \
        --server_tls_key_file=/certs/localhost.key \
        --backend_addr=localhost:8800 \
        --backend_tls_noverify
```
