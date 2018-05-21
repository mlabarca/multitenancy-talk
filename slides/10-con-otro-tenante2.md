$transition: fade$
## Cambiando el tenante

https://cliente1.nuestraapp.com
```
Apartment::Tenant.current
#=>
'cliente1'
```

```
class ApplicationController < ActionController::Base
  before_action :set_tenant_name

  def set_tenant_name
    @tenant_name = Apartment::Tenant.current
  end
end
```
