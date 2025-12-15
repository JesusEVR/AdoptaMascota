# Huellitas en Casa

**Huellitas en Casa** es una plataforma web diseñada para conectar mascotas que buscan un hogar con personas interesadas en adoptar. 
El objetivo principal es fomentar la adopción responsable y brindar una experiencia amigable y accesible para los usuarios.

---

## Tecnologías Utilizadas

- **Django REST Framework**
- **React + Vite**
- **TailwindCSS**
- **React Router DOM**
- **JavaScript (ES6+)**

---

## Integrantes del equipo — Gryffindor

- Anaya Pérez Ulises Josué (@ulisessap)
- Díaz Reyes Lilith Jaquelin (@jackDiazz)
- García López Francisco Daniel (@D-GaLo)
- García Velasco Erick Iram (@ErickSonico)
- Osorio Morales Fernanda Ameyalli (@FernandaOsorioMorales)
- Sautto Ramírez Seldon (@seldon1128)
- Tapia Sánchez Oscar (@OscarTapiaS)
- Vázquez Reyes Jesús Elías (@JesusEVR)

## Cómo ejecutar el proyecto

### Pasos para correr el Backend

La primera vez que corras el Backend, debes estar dentro de la carpeta Aplicacion:

```
cd Aplicacion
```

Una vez ahí, elimina la carpeta `venv`:

- En Windows (CMD)
    ```bash
    rmdir /s /q venv
    ```

- En Windows (PowerShell)
    ```bash
    Remove-Item -Recurse -Force venv
    ```

- En Linux / macOS
    ```bash
    rm -rf venv
    ```


Crea la carpeta nuevamente para tener un entorno virtual:

- En Windows (CMD/PowerShell)
    ```bash
    python -m venv venv
    ```

- En Linux / macOS
    ```bash
    python3 -m venv venv
    ```


Activa el entono virtual:

```bash
venv\Scripts\activate
```

Instala los requerimientos:

```bash
pip install -r requirements.txt
```

Ve al proyecto:

```bash
cd adopta_amigo
```

Haz las migraciones:

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

Crea un usuario administrador. Guarda los datos que vas a ingresar:

```bash
python manage.py createsuperuser
```

Inicia el servidor:

```bash
python manage.py runserver
```

Accede al panel de administración:

```
http://127.0.0.1:8000/admin/
```

En el panel, se te solicitarán datos del usuario administrador que creaste, después podrás consultar la información de la base de datos.

Cuando corras nuevamente el servidor, no es necesario eliminar y volver a crear la carpeta `venv`, ni tampoco generar un nuevo usuario admin.


### Pasos para correr el Frontend

Para ejecutar el frontend necesitamos abrir otra terminal y posicionarnos en la carpeta ```frontend``` del proyecto. Para ello, se ejecuta el siguiente comando:

```
cd AdoptaMascota/Aplicacion/frontend
```

Posteriomente, ponemos los siguientes comandos dentro de dicha carpeta:

```
npm install
```

```
npm run dev
```

Finalmente, se accede a ```http://localhost:5173/``` desde el navegador web para visualizar la aplicación.

### Detener procesos

Para dejar de correr todo se debe ejecutar ```Ctrl+C``` en ambas terminales, y para detener el entorno virtual del Backend debe ponerse el comando:

```
deactivate
```
