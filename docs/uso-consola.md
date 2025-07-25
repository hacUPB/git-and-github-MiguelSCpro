✅ 1. Crear el repositorio en GitHub (repositorio remoto)
Ve a https://github.com e inicia sesión.

Haz clic en el botón "New" o "Nuevo repositorio".

Asigna un nombre al repositorio.

(Opcional) Agrega una descripción.

Elige si será público o privado.

No marques la opción de "Initialize this repository with a README" si ya tienes un repositorio local.

Haz clic en "Create repository".

✅ 2. Crear el repositorio local (si no existe aún)
Abre la terminal y ve a la carpeta donde quieres tu proyecto:

bash
Copiar
Editar
cd ruta/del/proyecto
Inicializa Git:

bash
Copiar
Editar
git init
Agrega tus archivos al repositorio:

bash
Copiar
Editar
git add .
Haz tu primer commit:

bash
Copiar
Editar
git commit -m "Primer commit"
✅ 3. Conectar el repositorio local con el remoto
Copia la URL del repositorio remoto desde GitHub, puede ser algo así:

bash
Copiar
Editar
https://github.com/tu-usuario/nombre-del-repo.git
Luego, conéctalo desde la terminal:

bash
Copiar
Editar
git remote add origin https://github.com/tu-usuario/nombre-del-repo.git
Puedes verificar que se agregó correctamente con:

bash
Copiar
Editar
git remote -v
✅ 4. Enviar (push) los archivos locales al repositorio remoto
Si es tu primer "push", usa este comando para subir todo al repositorio remoto:

bash
Copiar
Editar
git push -u origin master
⚠️ Si estás usando una rama principal llamada main, reemplaza master por main:

bash
Copiar
Editar
git push -u origin main
✅ 5. Confirmar que todo está sincronizado
Ve a GitHub y actualiza la página del repositorio. Ahora deberías ver todos los archivos que tenías en tu repositorio local.
