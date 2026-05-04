# UF 1889
## Identificar modelos de clientes
- Clientes > res.partner (almacena clientes)
- Seguimientos -> mail.activity (almacena acticvidad)

### Modelos de clientes
res.partner

Campos utiles:
- `name`
- 'email`
- `phone`
- 'is_company`
- `customer_rank`

### Modelos de seguimientos
mail.activity

Campos utiles:
- `res_model`
- `res_id`
- `activity_type_id`
- `summary`
- `date_deadline`
- `user_id`
- `create_date`

### Relacion entre modelos
- En `mail.activity`, el registro apunta a un modelo y a un identificador
- cuando `res-model = 'res_partner'`, y `res_id`coincide con el id del cliente, esa pertenece a ese cliente.

### Decision funcional
Para estas practica se considera "cliente" a los registros del modelo `res.partner`con customer_rank > 0`, y `seguimiènto a los registros del modelo `mail.activity`asociados al cliente `res_model = 'res_partner' y res_id=< id del cliente>
