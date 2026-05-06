# Simulacion API
### Objectivo

Simular los datos que se podrian eviarse desde Odoo hacia otro sistema mediante un API 

### Endpoint simulado
```text
POST  /api/clientes/seguimientos
```

```json
[{
  "seguimiento_id": "",
  "fecha": "",
  "cliente": {
    "id": ,
    "nombre": "",
    "email": "@email.com",
    "telefono": "",
    "empresa": "",
    
  },
  "comercial": {
    "id": ,
    "nombre": "",
    "email": ""
  },
  "tipo_seguimiento": "",
  "estado": "completado",
  "resultado": "cliente interesado en propuesta premium",
  "proxima_accion": {
    "fecha": "",
    "tipo": "reunion",
    "descripcion": "Demo del producto"
  },
  "oportunidad": {
    "id": "OPP-9932",
    "nombre": "Venta software ERP",
    "etapa": "propuesta",
    "valor_estimado": ,
    "moneda": "EUR",
    "probabilidad": 
  },
  "notas": "Se discutieron funcionalidades avanzadas y tiempos de implementación.",
  "origen": "odoo_crm",
  "metadata": {
    "creado_en": "",
    "actualizado_en": "",
    "version": "1.0"
  }
}
]

o una api mas reducido

{
  "id": "SEG-145",
  "fecha": "",
  "cliente": {
    "id": 4821,
    "nombre": ""
  },
  "tipo": "llamada",
  "estado": "completado",
  "resultado": "Interesado",
  "proxima_fecha": ""
}

```json
[
    (
    "id":9,
    "complete:name":"Acme Corporation",
    "numero_seguimiento")
]




