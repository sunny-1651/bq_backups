# bq_backups

**centralized BQ Backup** *planned*
A python script which can run cloud function, cloud run or any other platform from which authentication to GCP can be established.
The destination of backup data can be either a snapshot table in BQ or a file (json, csv, avro, parquet) in gcs bucket.
Pre-req -> the backup dataset and or backup bucket to be pre-made.

