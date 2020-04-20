## UC: `OR-100` Create order

- Actors: `#Sales`
- Level: User goal
- Mockup: [Create order](#/orders/create)

### Main success scenario:

1. User enters order data.
2. User enters order item data.
3. System calculates the `Item total` for each item and `Invoice total` for the whole order.
4. User saves the order.
5. System validates the data.
6. System creates new `#Order`.
7. System sets `#Order.status` = `accepted`.
8. System sets `#Order.created` = current timestamp.
9. System sets `#Order.updated` = current timestamp.
10. System sets `#Order.orderNumber`  = `PO-YYYY-SSSSS`, where:
    - `PO` is a constant indicationg a purchase order
    - `YYYY` is the current year
    - `SSSSS` is a unique sequence number within the current year
11. System creates new `#OrderItem` for each order item created by the user.

### Extensions:

- 2a. User wants to order more than 1 item:
    - 2a1. User adds more item rows and fills them in.
- 2b. User wants to remove an item from the order:
    - 2b1. User deletes the item row.
- 5a. A required field is empty:
    - 5a1. System displays error: Required.
- 5b. [Due date](#Order.dueDate) is in past:
    - 5b1. System displays error: Must be in future.
- 5c. Item [unit price](#OrderItem.unitPrice) is < 0:
    - 5c1. System displays error: Must be >= 0.
- 5d. Item [quantity](#OrderItem.quantity) is <= 0:
    - 5d1. System displays error: Must be > 0.
