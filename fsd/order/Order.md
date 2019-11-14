## Entity: Order

### Attributes:

- Id (APK bigint)
- Version (M int) - Optimistic locking version
- Order number (M string 30)
- Customer id (FK `#Customer`)
- Due date (M date)
- Status (M enum: created, shipped, invoiced)
- Comment (O string)
- Created (M timestamp)
- Updated (M timestamp)
