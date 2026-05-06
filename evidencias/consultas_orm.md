# Consultas ORM
### Objectivo

Obtener el numero de seguimiento comerciales realizadas

##### Agrupar las actividades (mail.activity) por cliente (res_id)

```python
def _compute_activity_followup_count(self):
        # Agrupa las actividades (mail.activity) por cliente (res_id)
        grouped_data = self.env["mail.activity"].read_group(
            domain=[
                ("res_model","=","res.partner"),
                ("res_id","in",self.ids),
            ],
            fields=["res_id"],
            groupby=["res_id"],
        )

)