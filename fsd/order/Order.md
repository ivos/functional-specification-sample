## Entity: Order

### Attributes:

- Id (APK bigint): 1001
- Version (M bigint): 1 - Optimistic locking version
- Order number (M string 30): PO-2019-00035
- Customer (n:1 `#Customer`)
- Due date (M date): 2020-02-22
- Status (M enum: created, shipped, invoiced): `shipped`
- Comment (O string)
- Created (M timestamp): 2020-02-20T12:02:20.202
- Updated (M timestamp): 2020-02-22T20:20:02.020
- Order items (1:n `#OrderItem`)
