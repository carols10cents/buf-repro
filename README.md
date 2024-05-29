# `buf`+`import` = `file does not exist` issue reproduction

To reproduce:

```console
$ buf --version
1.32.2
$ git clone https://github.com/carols10cents/buf-repro.git
$ cd buf-repro
$ buf lint
Failure: bulk_ingester/protos/influxdata/iox/bulk_ingester/v1/progress.proto: import "generated_types/protos/influxdata/iox/column_type/v1/type.proto": file does not exist
```