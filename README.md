# Telegram AI Companion Bot

Bot de compañía y soporte emocional para Telegram, con respuestas en varios idiomas, alertas de error y capacidad de donación.

## ❤️ Qué hace
- Responde preguntas y conversa con el usuario.
- Envía contenido de ánimo y compañía.
- Permite recibir donaciones mediante enlaces.
- Envía alertas de error a administradores.

## ⚙️ Requisitos
- Python 3.10+
- Git
- Token de Telegram válido

## 🚀 Instalación
```powershell
cd D:\mejoras_portafolio\repos\telegram-ai-bot
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## 🔧 Configuración
Copia el archivo de ejemplo y configura tus variables:
```powershell
copy .env.example .env
```
Edita `.env` y completa:
- `TELEGRAM_TOKEN`
- `DONATION_URL` (opcional)
- `ADMIN_IDS`
- `LOG_LEVEL` (DEBUG, INFO, WARNING, ERROR)
- `LOG_FILE`
- `SENTRY_DSN` (opcional)

## ▶️ Ejecución
### Modo local
```powershell
python .\bot.py
```

### Modo Webhook
```powershell
python .\webhook_server.py
```

## 📌 Comandos disponibles
- `/start` – Iniciar conversación
- `/donar` o `/donate` – Mostrar enlace de donación
- `/help` – Mostrar ayuda en el idioma del usuario

## 🛡️ Seguridad
- No subas `TELEGRAM_TOKEN` a repositorios públicos.
- Usa `ADMIN_IDS` para controlar quién recibe alertas.
- Ajusta `LOG_LEVEL` y `LOG_FILE` para monitorear el bot.

## 🧠 Archivos importantes
- `bot.py` – entrada principal.
- `webhook_server.py` – servidor de webhook.
- `requirements.txt` – dependencias.
- `LICENSE` – licencia MIT.

## 📄 Licencia
Este proyecto está bajo licencia MIT.

