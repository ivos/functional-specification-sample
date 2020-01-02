## Entity: Customer

### Attributes:

- Id (APK bigint)
- Version (M bigint) - Optimistic locking version
- Name (M string 100)
- Tax number (OU string 14) - Min size 4
- Maturity interval (M int) - Invoice maturity interval [days], non-negative
- Mobile (C string 30)
- Email (C string 50)
- Web (O string 50)
- Updated (M timestamp)

### Notes

- Either `mobile` or `email` is required.
