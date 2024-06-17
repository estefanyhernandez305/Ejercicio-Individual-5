# Proyecto de Autenticación Django

## Objetivo
Este proyecto tiene como objetivo implementar una funcionalidad de login y logout en una aplicación web utilizando el framework Django. Incluye la restricción de acceso a ciertas vistas, asegurando que solo los usuarios autenticados puedan acceder.

## Funcionalidades
1. **Login**: Los usuarios pueden iniciar sesión con su nombre de usuario y contraseña.
2. **Logout**: Los usuarios pueden cerrar sesión.
3. **Restricciones de acceso**: 
   - Las vistas están protegidas para que solo los usuarios autenticados puedan acceder.
   - Se redirige automáticamente a la página de login si un usuario no autenticado intenta acceder a una vista protegida.

## Estructura de Templates
- `login.html`: Formulario de inicio de sesión.
- `home.html`: Página de inicio que muestra un mensaje de bienvenida con el nombre del usuario autenticado.

## Pasos para ejecutar el proyecto
1. Clonar el repositorio.
2. Crear un entorno virtual e instalar las dependencias.
3. Aplicar migraciones de la base de datos.
4. Ejecutar el servidor de desarrollo.

```bash
git clone <URL_DEL_REPOSITORIO>
cd mi_proyecto
python -m venv env
source env/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
