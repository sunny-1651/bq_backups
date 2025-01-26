# BQ TABLE SNAPSHOT

This is the way which i used only if the tables were created on fly and not in a planned way.
If we have table that are created systematically we can have a constructor that creates a table and also create a scheduled query to take backup snaps. [docs link](https://cloud.google.com/bigquery/docs/table-snapshots-scheduled)

The snapshots are taken such that there is a base snapshot and then the increamental snapshots have the changes w.r.t. to prev snap. The pricing is accordingly. [docs link](https://cloud.google.com/bigquery/docs/table-snapshots-intro#storage_costs)

