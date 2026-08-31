# Seafile-Collabora

Modificar datos en las líneas: 54, 55, 61 y 62

Línea 56, si lo crees conveniente, puedes generar una clave con este comando "openssl rand -base64 32"

-----------------------------

Si no has modificado los datos:

Ver en "http://localhost:8200" ó "seafile.tudominio.com"

Usuario: admin@example.com

Password: p4ssw0rd

------------------

Modifica el archivo seahub_settings.py  - Ruta: 

Añade estas líneas:

```
#Collabora Online
ENABLE_COLLABORA = True
COLLABORA_SERVER = 'https://collabora.dominio.com'
COLLABORA_SERVER_PORT = 9980
COLLABORA_SERVER_HTTPS = True
COLLABORA_FILE_SERVER_ROOT = 'https://app.midominio.com'
```

