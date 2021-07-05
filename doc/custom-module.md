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
<code>
    'installable': True,
</code>
<code>
    'application': True,
</code>
<code>
    'auto_install': False
</code>

4. Restart Server then update applist from odoo.
