## Cambiando el tenante

Manualmente:
```
Apartment::Tenant.switch('tenant_name') do
  # ...
end
```

Por consulta:

```
# config/application.rb
require 'apartment/elevators/subdomain' # or 'domain', 'first_subdomain', 'host'

#...
config.middleware.use Apartment::Elevators::Subdomain
```


