# DOCUMENTACION ADMNISTRACION REMOTA ASO EN WAC Y COCKPIT


## ***WINDOWS ADMIN CENTER (WAC)***

| Sistema administrado   | Herramienta           | Protocolo | Puerto |
|------------------------|-----------------------|-----------|--------|
| Windows Server 2025    | Windows Admin Center  | HTTPS     | 6600   |

### **WAC ACCESO**
![imagen1](Capturas/wac_acceso.png)

Aqui podemos ver que para meternos dentro del WAC, al ejecutar la aplicacion nos llevara la buscador para meter el usuario y la contraseña de la maquina que estamos utilizando. En la barra vemos la URL que hemos utilizado para entrar en el WAC, nombre del host:puerto.

### **WAC SERVIDOR**
![imagen1](Capturas/wac_servidor.png)

Una vez dentro de la WAC ahora tenemos que añadir el servidor a la WAC, para ello en agregar elegimos servidor y ponemos su direccion IP, despues elegimos entrar con creedenciales donde pondremos el usuario y contraseña administrador del servidor. Una vez añadido podremos ver que sale como servidor.


## ***COCKPIT***

| Sistema              | Usuario remoto | Herramienta | Protocolo | Puerto |
|----------------------|---------------|-------------|-----------|--------|
| Ubuntu Server 24.04  | usercockpit   | Cockpit     | HTTPS     | 9090   |
