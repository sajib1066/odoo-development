# Database setup for Odoo

Odoo needs a superuser for create database in postgresql.

1. Login Postgres
```
sudo -u postgres psql
```

2. Create Postgresql Super User for odoo
```
CREATE USER user_name SUPERUSER;
```

3. Set Password
```
\password user_name
```
