# Tetiva proto

Protobuf contracts for [Tetiva](https://tetiva.app) — the API definitions shared
by the desktop client and the sync server, plus generated Go code.

- `proto/` — `.proto` sources (managed with [buf](https://buf.build))
- `go/` — generated Go packages (`protoc-gen-go` / `protoc-gen-go-grpc`)

Regenerate with [Task](https://taskfile.dev): `task proto:gen`.

The protobuf package namespace (`gophercourier.*`) predates the Tetiva rename;
it stays as-is because service and message names are part of the wire protocol.

## License

[MIT](LICENSE)
