## Entity: Customer

### Attributes:

- Id (APK bigint): 1001
- Version (M bigint): 1 - Optimistic locking version
- Name (M string 100): Planet express
- Tax number (OU string 4 - 14): 01-9852145
- Maturity interval (M int >= 0): 30 - Invoice maturity interval in days
- Mobile (C string 30): 202-555-0182
- Email (C string 50): `info@planet-express.com`
- Web (O string 50): `https://planet-express.com`
- Updated (M timestamp): 2020-02-20T12:34:56.123

### Notes

- Either `mobile` or `email` is required.
