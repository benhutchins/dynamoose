# Breaking Changes

## 2.0 - incomplete list

- `scan.count()` has been removed, and `scan.counts()` has been renamed to `scan.count()`.
- Schema `default` value does not pass the model instance into `default` functions any more.
- `Model.update`
	- `$LISTAPPEND` has been removed, and `$ADD` now includes the behavior of `$LISTAPPEND`
	- `$DELETE` now maps to the correct underlying DynamoDB method instead of the previous behavior of mapping to `$REMOVE`
- `dynamoose.model` has been renamed to `dynamoose.Model`
- `dynamoose.local` has been renamed to `dynamoose.aws.ddb.local`
- `Model.getTableReq` has been renamed to `Model.table.create.request`
- `Model.table.create.request` (formerly `Model.getTableReq`) is now an async function