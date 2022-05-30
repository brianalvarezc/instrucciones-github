# instrucciones-github
## En github.com 
Instrucciones para poder hacer autenticación con personal access token desde git bash 

Primero se debe tener el personal access token (PAT) creado y guardado en alguna parte (si no, se debe regenerar para poderlo copiar y el acceso se pierde en las máquinas en donde esté autenticado)

- La creación del PAT se hace en la dirección: [https://github.com/settings/tokens](https://github.com/settings/tokens) o yendo desde la configuración principal del perfil de github, al final aparece unas opciones de desarrollador.
- Ya ubicado en las opciones de tokens,  se genera el nuebo token con el botón que lo indica.
- Aparece la pantalla de configuración de permisos del token, generalmente se deja así y si eres avanzado, asignarás los permisos y copiarás el token que aparece en la parte superior de la pantalla (Se debe copiar y asegurar porque no vuelve a aparecer y si se pierde, se debe regenerar y el anterior ya no sirve)
- Finalmente se hace en Actualizar o Crear token y listo, pasamos a git bash

## Git bash
Suponiendo que ya sabes el proceso de git clone, status, add, commit, etc etc continuamos a añadir el repositorio remoto para actualizar los cambios en https://github.com/*user-name*/*repository-name*.git

- Añadimos el repositorio remoto de la siguiente forma 
>git remote add origin https://**user-name**:**personal-access-token**@github.com/**user-name**/**repository-name**.git

Finalmente podemos enviar nuestros cambios al repo remoto con 
>git push origin **repository-branch**
