## Entity: Customer

### Attributes:

- Id (APK bigint)
- Version (M int) - Optimistic locking version
- Name (M string 100)
- Tax number (OU string 14)
- Maturity interval (M int) - Invoice maturity interval [days]
- Mobile (C string 30)
- Email (C string 50)

### Notes

- Either `mobile` or `email` is required.
