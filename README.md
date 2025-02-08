 🔧 Instalación y ejecución  

1️⃣ Clonar el repositorio  
```bash
git clone <URL_DEL_REPO>
cd crud_tareas
```

---

2️⃣ Configurar el Backend  

📍 Ir a la carpeta del backend**  
```bash
cd backend
```

📍 Instalar dependencias**  
```bash
npm install
```

📍Configurar variables de entorno**  
Crea un archivo **.env** en la carpeta `backend` con el siguiente contenido:  
```
MONGO_URI=mongodb://localhost:27017/tareas_db
JWT_SECRET=clave_secreta_para_jwt
PORT=5000
```

Ejecutar el servidor**  
```bash
npm start
```
El backend se ejecutará en `http://localhost:5000`.


3️⃣ Configurar el Frontend  

📍 Ir a la carpeta del frontend**  
```bash
cd ../frontend
```

📍 **Instalar dependencias**  
```bash
npm install
```

📍 Ejecutar la aplicación**  
```bash
npm run dev
```
El frontend se ejecutará en `http://localhost:5173`.

---

📌 Endpoints del Backend  

| Método  | Ruta                  | Descripción                | Autenticación |
|---------|-----------------------|----------------------------|--------------|
| POST    | `/api/auth/register`  | Registro de usuario       | ❌ |
| POST    | `/api/auth/login`     | Inicio de sesión          | ❌ |
| GET     | `/api/tareas`         | Obtener todas las tareas  | ✅ |
| POST    | `/api/tareas`         | Crear una nueva tarea     | ✅ |
| PUT     | `/api/tareas/:id`     | Editar una tarea          | ✅ |
| DELETE  | `/api/tareas/:id`     | Eliminar una tarea        | ✅ |
