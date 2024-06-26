# Sistema bajo prueba: ParaBank
## Objetivo

### Pruebas front-end:
* Registro
  * Haga click en <Registro>
  * Rellene el formulario de registro con los datos requeridos
  * Pulse de nuevo en <Registro>.
  * Compruebe que el texto "Su cuenta se ha creado correctamente." En la pantalla se puede ver "You are now logged in."
* Abrir una cuenta nueva
  * Haga click en <Abrir nueva cuenta>
  * En el apartado "¿Qué tipo de cuenta desea abrir?" seleccione la opción <SAVINGS>.
  * Haga clic en <Abrir nueva cuenta>
  * Compruebe si el texto "Congratulations, your account is now open." está visible en la pantalla
* Resumen de las cuentas
  * Haga clic en <Resumen de cuentas>
  * Compruebe si el texto "*El saldo incluye depósitos que pueden estar sujetos a retenciones" está visible en la pantalla
* Transferir Fondos
  * Haga clic en <Transferencia de fondos>
  * Compruebe que el texto "Transferir fondos" es visible en la pantalla
  * En el campo <Importe: $> introduzca el importe a transferir
  * En el campo <De la cuenta #> seleccione una cuenta
  * En el campo <a la cuenta #> seleccione una cuenta distinta a la anterior
  * Haga clic en <Transferencia>
  * Compruebe que el texto "¡Transferencia completa!" es visible en la pantalla
* Actividad de la cuenta (cada mes)
  * Haga clic en <Resumen de cuentas>
  * Compruebe que el texto "*El saldo incluye depósitos que pueden estar sujetos a retenciones" es visible en la pantalla
  * Haga clic en una cuenta en la columna <Cuenta>.
  * Compruebe que el texto "Detalles de la cuenta" es visible en la pantalla
  * En "Actividad de la cuenta" haga clic en <Periodo de actividad:> y seleccione "Todo"
  * En "Actividad de la cuenta" haga clic en <Tipo:> y seleccione "Todo"
  * Haga clic en <Ir>

### Prueba back end de la API Rest:
* Validación del código de estado 200 para todas las etapas de las pruebas frontales
* Registro URL: https://parabank.parasoft.com/parabank/register.htm
* Abrir una nueva cuenta URL: https://parabank.parasoft.com/parabank/services_proxy/bank/createAccount?customerId=12545&newAccountType=1&fromAccountId=xxxxx
* Resumen de las cuentas URL: https://parabank.parasoft.com/parabank/overview.html
* Descarga de fondos URL: https://parabank.parasoft.com/parabank/services_proxy/bank/transfer?fromAccountId=13566&toAccountId=13677&amount=xxxxx
* Actividad de la cuenta (cada mes) URL: https://parabank.parasoft.com/parabank/services_proxy/bank/accounts/13566/transactions/month/All/type/All# paraBank-automation
