# Changelog

## 0.5.0

- Add high-level API via Manager class
- Add support for MySQL
- Auto-connect is performed for async queries if database is initialized, so no need to call `connect_async()` manually! And no worries, nothing will happen on duplicate calls

## 0.4.1

- Fixing critical transactions issues, see #12
- Internal `SELECT` query executor rewritten, got rid of some hacks
- Deferred database init is supported

## 0.4.0

- Add `db.atomic_async()` context manager to support transactions. Thanks, @mrbox!

## 0.3.4

- Fix: cursor is released back to connection pool after SQL execution error

## 0.3.3

- Add public `allow_sync` flag to database class, `True` by default
- Remove arguments from `sync_unwanted()` context manager function
- Add autodocs on `peewee_asyncext`

## 0.3

- #7, fixed bug with empty result after inserting row with UUID pk 
- some missing tests added
