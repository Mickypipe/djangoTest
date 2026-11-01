# Reservas, prueba con Django

Proyecto de práctica de Django 5.2 iniciado en noviembre de 2025, en desarrollo.

## Cómo correrlo

1. Crear y activar el entorno virtual:

   ```
   python -m venv .venv
   .venv\Scripts\activate
   ```

2. Instalar Django:

   ```
   pip install django
   ```

3. Copiar `.env.example` a `.env` y generar una clave para `DJANGO_SECRET_KEY`:

   ```
   copy .env.example .env
   python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
   ```

4. Migrar y levantar el servidor:

   ```
   python manage.py migrate
   python manage.py runserver
   ```

Autor: Miguel Angel Silva Pascua
