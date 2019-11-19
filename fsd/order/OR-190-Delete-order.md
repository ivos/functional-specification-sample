## UC: `OR-190` Delete order

- Actors: `#Sales`
- Level: User goal
- Mockup: [Order detail](#/orders/detail)

### Main success scenario:

1. User finds order in `#Order.status` `created`.
2. User deletes the order.
3. System validates the data.
4. System deletes all `#OrderItem`s of the order and the `#Order` itself.

### Extensions:

- 3a. `#Order.status` is not `created`:
    - 3a1. System displays error: Invalid status.
