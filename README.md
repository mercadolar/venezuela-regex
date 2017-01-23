# Regular expressions common when validating data related to Venezuela.
## Expresiónes regulares para validar data relacionada a Venezuela.

### ID document - Cédula de Identidad
```javascript
/^[V|E|J|P][0-9]{5,9}$/
```

### Date in the day/month/year format - Fecha en el formato día/mes/año
```javascript
/^(((0[1-9]|[12]\d|3[01])\/(0[13578]|1[02])\/((19|[2-9]\d)\d{2}))|((0[1-9]|[12]\d|30)\/(0[13456789]|1[012])\/((19|[2-9]\d)\d{2}))|((0[1-9]|1\d|2[0-8])\/02\/((19|[2-9]\d)\d{2}))|(29\/02\/((1[6-9]|[2-9]\d)(0[48]|[2468][048]|[13579][26])|((16|[2468][048]|[3579][26])00))))$/
```

### Bank account number - Número de cuenta bancaria
* Always 20 digits.
* First 4 are the bank's ID (see [bcv.org.ve's official list](http://www.bcv.org.ve/snp/instcce.pdf))
and the following 15 are the account number.
* This regex validates there are 20 continuous digits and groups the match in two.


* Siempre 20 dígitos.
* Los primeros 4 son el código del banco (ver [lista oficial del bcv.org.ve](http://www.bcv.org.ve/snp/instcce.pdf))
y los 15 siguientes son el número de cuenta.
* Este regex valida que hay 20 dígitos continuous y agrupa el encuentro en dos.

```javascript
/^(\d{5})(\d{15})$/
```
