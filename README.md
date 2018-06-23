# merkle-stamp
Toolkit for verifying consistency of assets

## Applications include

### Event stream integrity

Source sends X events, Sink receives Y events
Check that X == Y and events are not lost in transit


### Database integrity

1) Database in state X, code release happens, code rollback happens, database in state Y
Check that X == Y and rollback was a success

2) Database in state X on environment A, release code to environment B, dataase in state Y
Check that X == Y and code release was a success


### Directory integrity

Filesystem directory in state X on day 1, Filesystem directory in state Y on day 2
Check that X == Y and directory has not been corrupted


### Subresource integrity

Webserver is serving n assets in state X on day 1, Webserver is serving n assets in state Y on day 2
Check that X == Y and assets are not corrupted