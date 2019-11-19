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

### Extensions:

- 2a. User wants to order more than 1 item:
    - 2a1. User adds more item rows and fills them in.
- 2b. User wants to remove an item from the order:
    - 2b1. User deletes the item row.
- 5a. A required field is empty:
    - 5a1. System displays error: Required.
- 5b. [Due date](#Order.dueDate) is in past:
    - 5b1. System displays error: Must be in future.
- 5c. Item [unit price](#OrderItem.unitPrice) or [quantity](#OrderItem.quantity) is <= 0:
    - 5c1. System displays error: Must be > 0.
