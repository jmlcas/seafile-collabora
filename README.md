# Seafile-Collabora

Modificar datos en las líneas: 58, 59, 65, 66, 82 y 83

Línea 56, si lo crees conveniente, puedes generar una clave con este comando "openssl rand -base64 32"

Cambiar: 

seafile.tudominio.com por el dominio ó subdominio real que uses

collabora.tudominio.com por el dominio ó subdominio real que uses

-----------------------------

Si no has modificado los datos:

Ver en "https://seafile.tudominio.com"

Usuario: admin@example.com

Password: p4ssw0rd

------------------

Modifica el archivo seahub_settings.py  - Ruta: /root/docker/seafile-collabora/opt/seafile-data/seafile/conf/seahub_settings.py

Añade estas líneas, pero modifica tudominio.com

```
#Collabora Online
OFFICE_SERVER_TYPE = 'CollaboraOffice'
ENABLE_ONLYOFFICE = False
ENABLE_OFFICE_WEB_APP = True
OFFICE_WEB_APP_BASE_URL = 'https://collabora.tudominio.com/hosting/discovery'
WOPI_ACCESS_TOKEN_EXPIRATION = 30 * 60
OFFICE_WEB_APP_FILE_EXTENSION = ('odp', 'ods', 'odt', 'xls', 'xlsb', 'xlsm', 'xlsx','ppsx', 'ppt', 'pptm', 'pptx', 'doc', 'docm', 'docx')
ENABLE_OFFICE_WEB_APP_EDIT = True
OFFICE_WEB_APP_EDIT_FILE_EXTENSION = ('odp', 'ods', 'odt', 'xls', 'xlsb', 'xlsm', 'xlsx','ppsx', 'ppt', 'pptm', 'pptx', 'doc', 'docm', 'docx')
```
