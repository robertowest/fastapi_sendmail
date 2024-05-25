# Email API

Esta es una API simple para enviar correos electrónicos utilizando FastAPI y `smtplib`.

## Instalación

1. Clona el repositorio:
```bash
git clone <URL_DEL_REPOSITORIO>
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
```

3. Configura las variables de entorno en el archivo `.env`

## Ejecución

Ejecuta la aplicación con uvicorn:
```bash
uvicorn main:app --reload
```

La API estará disponible en `http://127.0.0.1:8000`

## Endpoints

`POST /send-email/`: envía un correo electrónico. El cuerpo de la solicitud debe ser un JSON con el formato:
```json
{
    "subject": "Asunto del mensaje",
    "recipients": ["persona1@corre.com","persona2@correo.com"],
    "body": "Cuerpo del mensaje"
}
```

