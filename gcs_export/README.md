# GCS EXPORT 

An excerpt from documentation to decide the file type for export.
This kind of backup is generally for master backup, usually tested in dev env, deployed in prd and skipped for all other envs.

Data format | Supported compression types | Details
CSV | GZIP | You can control the CSV delimiter in your exported data by using the --field_delimiter bq command-line tool flag or the configuration.extract.fieldDelimiter extract job property. *Nested and repeated data is not supported.*
JSON | GZIP | *Nested and repeated data are supported.*
Avro | DEFLATE, SNAPPY | GZIP is not supported for Avro exports. *Nested and repeated data are supported.*
Parquet | SNAPPY, GZIP, ZSTD | *Nested and repeated data are supported.*

