RUST_LOG=info cargo run --release --bin jito-shredstream-proxy -- shredstream \
 --src-bind-port 4010 \
 --grpc-service-port 8000
