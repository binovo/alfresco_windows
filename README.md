# Ansible Windows

Instalador para Alfresco Community versión 6.2, sobre equipos basados en Windows donde no se recomienda ejecutar contenedores todavía.

## Instrucciones:

En el servidor solamente es necesario configurar el sistema de WinRM, agregando un "listener" que nos permita realizar la conexión desde Ansible. Esto es solamente necesario para el proceso de instalación, y puede ser removido al finalizar el proceso.

### En el servidor:

1. Descargar:
https://github.com/ansible/ansible/blob/devel/examples/scripts/ConfigureRemotingForAnsible.ps1

2. Desde powershell ejecutar:

```
$username = Administrator
$password = 'greencore123queso'
.\ConfigureRemotingForAnsible.ps1
```


### Equipo controlador
