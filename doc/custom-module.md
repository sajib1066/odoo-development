# Custom Module Development

Odoo has lot of default module. But we need some custom module for our specific projects. Odoo default module located in addons directory.
We can create new directory for our custom module.

1. Create New Directory for Custom Module
```
mkdir custom
```

2. Create New Custom Module on Custom module directory
```
python odoo-bin scaffold <module_name> custom/
```

3. Check the __manifest__.py file and add some configurations
```
'installable': True,
'application': True,
'auto_install': False
```

4. Restart Server then update applist from odoo.

5. Adding Custom Icon
Create a static directory into the module directory then create a description into static. Then put the icon image into the description directory named icon.png
