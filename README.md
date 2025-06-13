# Script de extracción diaria Samsara

## Requisitos
- Python 3.9 o superior (ideal 3.10+)
- SQL Server con tabla `Eventos_Samsara`
- Tener configurado el archivo `.env` en la raíz con tus credenciales y token

## Instalación
1. Clona el repo
2. Instala dependencias:
    pip install -r requirements.txt
3. Configura el archivo `.env` (usa el ejemplo proporcionado)
4. Ejecuta manualmente con:
    python tu_script.py

## Para automatizar con Task Scheduler:
- Programa el .py o un .bat que llame:
    python ruta\al\script.py

## Variables del .env
- SAM_AUTH: token Bearer de Samsara (incluye la palabra Bearer)
- SQL_SERVER: IP o nombre del servidor SQL
- SQL_DB: nombre de la base de datos
- SQL_USER: usuario de la base
- SQL_PASS: contraseña
- CONFIG_ID: configurationId de alertas
