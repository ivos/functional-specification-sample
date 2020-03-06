## Entity: Customer

### Attributes:

- Id (APK bigint)
- Version (M bigint) - Optimistic locking version
- Name (M string 100)
- Tax number (OU string 4 - 14)
- Maturity interval (M int >= 0) - Invoice maturity interval in days
- Mobile (C string 30)
- Email (C string 50)
- Web (O string 50)
- Updated (M timestamp)

### Notes

- Either `mobile` or `email` is required.
