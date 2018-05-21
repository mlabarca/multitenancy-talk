## Gema Apartment

https://github.com/influitive/apartment

* Una sola base de datos, múltiples schemas de PostgreSQL.
* Permite específicar los tenantes estáticamente un archivo de configuración:

```
# config/apartment.rb
config.tenant_names = %w[cliente1 cliente2]
```

O crearlos dinámicamente en cualquier momento:
```
Apartment::Tenant.create('tenant_name')
```
