1. Crear un repositorio remoto en GitHub
🔹 Paso 1: Inicia sesión en https://github.com
🔹 Paso 2: Crea un nuevo repositorio
Haz clic en el botón “New repository” (o "+" > New repository).

Ponle un nombre, por ejemplo: mi_proyecto.

Puedes añadir una descripción (opcional).

Elige si quieres que sea público o privado.

⚠️ No marques ninguna casilla extra (ni README, ni .gitignore, si ya lo tienes local).

Haz clic en "Create repository".

💻 2. Conectar el repositorio local al remoto
Asumiendo que ya tienes un repositorio local inicializado con git init (como te expliqué antes), ahora lo vas a enlazar con GitHub.

🔹 Paso 3: Copia la URL del repositorio remoto
Por ejemplo:

arduino
Copiar código
https://github.com/tuusuario/mi_proyecto.git
O si usas SSH:

scss
Copiar código
git@github.com:tuusuario/mi_proyecto.git
🔹 Paso 4: Añade el repositorio remoto al local
Desde la carpeta del proyecto en tu consola:

bash
Copiar código
git remote add origin https://github.com/tuusuario/mi_proyecto.git
💡 Esto le dice a Git que "origin" será el nombre del repositorio remoto.

🔹 Paso 5: Sube tu proyecto a GitHub
bash
Copiar código
git push -u origin main
⚠️ Si tu rama principal se llama master, usa master en lugar de main:

bash
Copiar código
git push -u origin master
📌 La primera vez usamos -u para que Git recuerde qué rama está enlazada con cuál.

✅ A partir de ahí...
Cada vez que hagas cambios y commits locales, puedes sincronizar con:

bash
Copiar código
git push
Y si trabajas en otro equipo o desde otro PC, puedes traer los cambios con:

bash
Copiar código
git pull
🔁 Resumen del flujo completo
bash
Copiar código
# Ya dentro de tu carpeta del proyecto
git init
git add .
git commit -m "Primer commit"

# Conecta con GitHub (URL según sea HTTPS o SSH)
git remote add origin https://github.com/tuusuario/mi_proyecto.git

# Sube todo al repositorio remoto
git push -u origin main
