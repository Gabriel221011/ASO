
# Práctica 2 – UT4  
## Administración remota de sistemas en red  
**Curso 2025/2026 – ASO**

## Infraestructura utilizada

- **Servidor Linux:** Ubuntu Server 24.04  
- **Servidor Windows:** Windows Server 2025  
- **Equipo administrador:** Windows 11  
- **Red:** Red privada  
- **Cliente SSH:** PuTTY  
- **Protocolo gráfico remoto:** RDP  

Todas las conexiones se realizan desde el equipo **Windows 11**.

## Parte 1 – Acceso remoto seguro por SSH

### Configuración realizada

- **Servicio:** SSH  
- **Servidor:** Ubuntu Server 24.04  
- **Usuario autorizado:** `remoto_ssh`  
- **Cliente:** PuTTY (Windows 11)  
- **Autenticación:** Clave pública  
- **Acceso por contraseña:** Deshabilitado  
- **Usuarios no autorizados:** Acceso denegado  

La conexión SSH se realiza exclusivamente mediante clave pública, utilizando un usuario dedicado creado únicamente para este propósito.

### Evidencias

1.	Usuario creado

![imagen1](Capturas/usuario_creado.png)
   
3.	Servicio SSH activo

![imagen1](Capturas/ssh_activo.png)

4.	Claves generadas. Captura donde se vean las claves generadas en el directorio final con los permisos adecuados.

![imagen1](Capturas/claves_generadas.png)

Publica

![imagen1](Capturas/clave_publica.png)

Privada

![imagen1](Capturas/clave_privada.png)

5.	Acceso por contraseña deshabilitado.

![imagen1](Capturas/acceso_contraseña_deshabilitado.png)

7.	Acceso SSH desde PuTTY con remoto_ssh.

![imagen1](Capturas/acceso_a_ubuntu_desde_putty_con_remoto.png)

8.	Acceso denegado a otro usuario. Captura del intento fallido con un usuario distinto de remoto_ssh.

![imagen1](Capturas/acceso_denegad.png)


## Parte 2 – Administración remota gráfica (RDP)

### Configuración realizada

- **Sistema administrado:** Windows Server 2025  
- **Protocolo:** RDP  
- **Usuario RDP:** `remoto_rdp`  
- **Grupo de acceso:** Usuarios de Escritorio remoto  
- **Autenticación de nivel de red (NLA):** Habilitada  
- **Cifrado:** Sí  
- **Usuarios no autorizados:** Acceso denegado  

El acceso remoto gráfico se realiza únicamente mediante un usuario dedicado, con control explícito de permisos y seguridad reforzada mediante NLA.

### Evidencias

1.	Usuario remoto_rdp creado y añadido al grupo. Captura donde se vea el usuario dentro del grupo Usuarios de Escritorio remoto.

![imagen1](Capturas/remoto_ssh_creado_y_añadido_a_grupo.png)

2.	Autenticación de nivel de red para la conexión habilitada.

![imagen1](Capturas/NAL_habilitada.png)

3.	Sesión RDP activa donde se vea escritorio del servidor y usuario remoto_rdp conectado.

![imagen1](Capturas/conexion_rdp_remoto.png)

4.	Acceso denegado a otro usuario. Captura del intento fallido con un usuario distinto de remoto_rdp.


