## Screen: Create order `/orders/create`

> UC: `#OR-100`

### Form: Order

- Order number (RO): PO-2019-00037
- Customer (R select: Cookieville Minimum Security Orphanarium, Democratic Order of Planets, MomCorp, Planet express)
- Due date (R date)
- Comment (multiLine)

### Table: Order items

- Product (R select: Cigar, Pabst Blue Robot beer 6-pack, BendërBrau ColdFusion Stream Beer Premium)
- Unit price (R text)
- Quantity (R text)
- Item total
    - 0
- Delete row
    - [warning: <i class="far fa-trash-alt"></i>]()

[:<i class="fas fa-plus"></i> Add row]()

Invoice total: 0

### Form:

[primary: <i class="fas fa-check"></i> Save](#/orders/detail)

> Creates `#Order` record and its `#OrderItem` records.

[:<i class="fas fa-chevron-left"></i> Back](#/orders)
