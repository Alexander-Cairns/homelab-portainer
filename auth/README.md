# Auth

Authentication stack based on lldap, and authelia.

# Configuration

The following enviroment variables are required to be configured.

- `LLDAP_JWT_SECRET`: Random password
- `LLDAP_KEY_SEED`: Random password
- `LLDAP_LDAP_USER_PASS`: Random password
- `SMTP_HOST`: `smtp.fastmail.com`
- `SMTP_PORT`: `465`
- `LLDAP_SMTP_OPTIONS__SMTP_ENCRYPTION`: `TLS`
- `SMTP_USER`: smtp authentication user
- `SMTP_PASSWORD`: smtp authentication password
- `LLDAP_SMTP_OPTIONS__FROM`: `example.com ldap no reply <no-reply+smtp@example.com>`
- `LLDAP_SMTP_OPTIONS__TO`: `example.com auth <auth@example.com>`
- `AUTHELIA_BIND_PASSWORD`: Ramdomly generated password
- `AUTHELIA_IDENTITY_VALIDATION_RESET_PASSWORD_JWT_SECRET`: 64 character plus generated string
- `AUTHELIA_SESSION_SECRET`: 64 character plus generated string
- `AUTHELIA_STORAGE_ENCRYPTION_KEY`: 64 character plus generated string
