# protos

protos define shared proto pkg for all golang repos.

## File generation

protos:
```
make protos
```

## Single file generation example

```shell
protoc --proto_path=. --go_out=paths=source_relative:. --go-grpc_out=paths=source_relative:.
      pkg/proto/gateway/v2/analytics.proto
```

faker:
```
make faker
```

## Usage

To use protos in another repo, add
`github.com/myDevicesIoT/protos v1.0.7` to go.mod file.