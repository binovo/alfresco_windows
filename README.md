# Ansible Windows

Instalador para Alfresco Community versión 6.2, sobre equipos basados en Windows donde no se recomienda ejecutar contenedores todavía.

## Instrucciones:

En el servidor solamente es necesario configurar el sistema de WinRM, agregando un "listener" que nos permita realizar la conexión desde Ansible. Esto es solamente necesario para el proceso de instalación, y puede ser removido al finalizar el proceso.

### En el servidor:
1. Desde powershell ejecutar:

```
Invoke-WebRequest -Uri https://raw.githubusercontent.com/ansible/ansible/devel/examples/scripts/ConfigureRemotingForAnsible.ps1 -OutFile ConfigureRemotingForAnsible.ps1
$username = "Administrator"
$password = "gr33nc0r3."
.\ConfigureRemotingForAnsible.ps1
```

### Equipo controlador

1. Actualizar el IP del equipo en inventory/hosts.ini
   Si lo ejecuta desde WSL, puede utilizar localhost

2. Ejecutamos receta de ansible. Dura algunos minutos mientras descarga e instala los diversos componentes.

```
ansible-playbook -i inventory/hosts.ini instalador_alfresco.yml
```

