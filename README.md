# seafile
Seafile -  Servidor archivos - Docker compose

Ver en "localhost:8200"

Usuario: me@example.com 

Password: asecret    

# Integración con ONLYOFFICE

Después de instalar Seafile deberemos editar el archivo "seahub_settings.py" en nuestro servidor. Ruta: /seafile/opt/seafile-data/seafile/conf/

La última línea sirve para conectar con OnlyOffice Desktop 

-Enable Only Office-

ENABLE_ONLYOFFICE = True

VERIFY_ONLYOFFICE_CERTIFICATE = False  #True

ONLYOFFICE_APIJS_URL = 'http{s}://{your OnlyOffice server's domain or IP}/web-apps/apps/api/documents/api.js'

ONLYOFFICE_FILE_EXTENSION = ('doc', 'docx', 'ppt', 'pptx', 'xls', 'xlsx', 'odt', 'fodt', 'odp', 'fodp', 'ods', 'fods')

ONLYOFFICE_EDIT_FILE_EXTENSION = ('doc', 'docx', 'ppt', 'pptx', 'xls', 'xlsx')

ONLYOFFICE_JWT_SECRET = 'my_secret'

ONLYOFFICE_FORCE_SAVE = True

ONLYOFFICE_DESKTOP_EDITORS_PORTAL_LOGIN = True

