## Screen: Order detail `/orders/detail`

### ReadOnlyForm: Order

- Order number: PO-2019-00035
- Customer: [Planet express](#/customers/detail)
- Status: Created
- Due date: in 2 days (14. 11. 2019)
- Comment: The cigars better not be too dry!
- Created: 2 days ago (8. 11. 2019 15:35)
- Updated: an hour ago (10. 11. 2019 9:51)
- [:Edit](#/orders/edit)
- [:Ship]()

> Enabled in `#Order.status` `created`. Sets `#Order.status` to `shipped`.

- [:Invoice]()

> Enabled in `#Order.status` `shipped`. Sets `#Order.status` to `invoiced`.

- [:Back](#/orders)
- [:Delete]()

> Enabled in `#Order.status` `created`. Toggles the delete panel below. The panel is hidden by default.

- FieldSet: Delete order confirmation
    - [danger: Confirm]() deleting this order.

    > Enabled in `#Order.status` `created`.\
    > UC: `#OR-190`

### Table: Order items

- Product
    - Cigar
    - Pabst Blue Robot beer 6-pack
    - BendërBrau ColdFusion Stream Beer Premium
- Unit price
    - 2.35
    - 3.24
    - 3.49
- Quantity
    - 8
    - 1
    - 4
- Item total
    - 18.8
    - 3.24
    - 13.96

Invoice total: 36
