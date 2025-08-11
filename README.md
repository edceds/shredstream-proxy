- Receive shreds on UDP port, parse, and start server
  RUST_LOG=info cargo run --release --bin jito-shredstream-proxy -- shredstream \
   --src-bind-port 4010 \
   --grpc-service-port 8000

src-bind-port = UDP port you'll receive shreds
grpc-service-port = port for starting a server to send shreds to clients

- Connect to the server using https://github.com/ValidatorsDAO/solana-stream#readme
