# Regular expressions common when validating data related to Venezuela.
## Expresiónes regulares para validar data relacionada a Venezolana.

### ID document - Cédula de Identidad
```javascript
/^[V|E|J|P][0-9]{5,9}$/
```

### Date in the day/month/year format - Fecha en el formato día/mes/año
```javascript
/^(((0[1-9]|[12]\d|3[01])\/(0[13578]|1[02])\/((19|[2-9]\d)\d{2}))|((0[1-9]|[12]\d|30)\/(0[13456789]|1[012])\/((19|[2-9]\d)\d{2}))|((0[1-9]|1\d|2[0-8])\/02\/((19|[2-9]\d)\d{2}))|(29\/02\/((1[6-9]|[2-9]\d)(0[48]|[2468][048]|[13579][26])|((16|[2468][048]|[3579][26])00))))$/
```