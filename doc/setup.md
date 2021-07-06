# How to Setup Odoo

1. Clone Odoo Source Code
```
git clone git@github.com:odoo/odoo.git
```

2. Go to odoo directory
```
cd odoo/
```

3. Create Virtualenv
```
python3 -m venv venv
```

4. Active Virtualenv
```
source venv/bin/activate
```

5. Install requirements
```
pip install -r requirements.txt
```

6. Make configuration file
```
cp debian/odoo.conf odoo.conf
```
```
[options]
; This is the password that allows database operations:
admin_passwd = <master_password>
db_host = <db_host>
db_port = <db_port>
db_user = <db_user>
db_password = <db_password>
xmlrpc_port = 8000
addons_path = <addons_directory_path>,
```

7. Run Server
```
python odoo-bin -c odoo.conf
```

Go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
