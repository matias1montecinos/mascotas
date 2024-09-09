# Manual GitHub:

## 1. Crear el repositorio en GitHub:
   - Ve a GitHub (https://github.com/) y inicia sesión.
   - Haz clic en el botón "+" en la esquina superior derecha y selecciona "New repository".
   - Nombra el repositorio como "mi-app-repository".
   - Asegúrate de que sea público (a menos que tengas una cuenta pro y quieras que sea privado).
   - No inicialices el repositorio con un README, .gitignore o licencia.
   - Haz clic en "Create repository".

## 2. Inicializar el repositorio Git local (si aún no lo has hecho):
   Abre una terminal en el directorio raíz de tu proyecto y ejecuta:
   ```
   git init
   ```

## 3. Crear el archivo .gitignore:
   Crea un archivo `.gitignore` en el directorio raíz del proyecto con el siguiente contenido:

```text
# Python
__pycache__/

# Virtual Environment
venv/
env/

# Flask
instance/
.webassets-cache

# Logs
*.log

# Database
*.sql

# Environment variables
.env

# IDE specific files
.vscode/
.idea/
```

## 4. Agregar los archivos al staging area:
   ```
   git add .
   ```

## 5. Realizar el primer commit:
   ```
   git commit -m "Initial commit: Flask app "
   ```

## 6. Conectar tu repositorio local con el remoto:
   ```
   git remote add origin https://github.com/your-user/your-repository.git
   ```

## 7. Verificar que el remote se haya agregado correctamente:
   ```
   git remote -v
   ```
   Deberías ver algo como:
   ```
   origin  https://github.com/your-user/your-repository.git(fetch)
   origin  https://github.com/your-user/your-repository.git (push)
   ```

## 8. Establecer la rama principal:
   ```
   git branch -M main
   ```

## ##9. Subir los cambios al repositorio remoto:
   ```
   git push -u origin main
   ```

Si es la primera vez que haces push a GitHub desde tu máquina, es posible que te pida autenticarte. En ese caso, sigue las instrucciones en pantalla para autenticarte.

## 10. Verifica que los cambios se hayan subido:
    Ve a https://github.com/your-user/your-repository.git y deberías ver tus archivos allí.

Estos pasos deberían permitirte crear el repositorio en GitHub y subir tu proyecto exitosamente. Si encuentras algún problema en alguno de estos pasos, por favor házmelo saber y te ayudaré a resolverlo.