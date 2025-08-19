

### **Frontend (Cliente)**
* **HTML5 y CSS3:** Para la estructura y el estilo base de la web.
* **Bootstrap:** Framework de CSS para un diseño responsive y componentes pre-diseñados.
* **React (con Vite):** Biblioteca para construir interfaces de usuario interactivas y rápidas.
* **Fetch API:** Para realizar las peticiones HTTP a nuestro backend.

### **Backend (Servidor)**
* **Python:** Lenguaje de programación principal del lado del servidor.
* **Flask:** Micro-framework para construir nuestra API REST de forma ligera y eficiente.
* **SQLAlchemy:** ORM para interactuar con la base de datos usando objetos de Python.
* **PostgreSQL / SQLite:** Nuestro sistema de gestión de bases de datos relacionales.
* **Flask-JWT-Extended:** Para manejar la autenticación de usuarios mediante JSON Web Tokens (JWT).
* **Flask-Migrate:** Para gestionar las migraciones y cambios en el esquema de la base de datos.

### **Herramientas de Desarrollo y Colaboración**
* **Git y GitHub:** Para el control de versiones y el repositorio centralizado del código.
* **GitHub Projects:** Herramienta para la gestión de tareas, sprints y seguimiento del progreso del equipo (metodología ágil).
* **VS Code:** Nuestro editor de código principal.
* **Postman:** Para probar los endpoints de nuestra API REST.
* **Figma:** Para diseñar los wireframes, mockups y prototipos de la interfaz de usuario.
* **whatsapp:** Nuestro canal de comunicación oficial para el equipo.
* **Google Docs:** Para la documentación colaborativa del proyecto.

### **Despliegue (Deployment)**
* **Backend:** Desplegado en **Render**.
* **Frontend:** Desplegado en **Vercel**.

### **APIs y Servicios Externos**
* **Mapbox:** Para integrar mapas interactivos en nuestra aplicación (si es necesario).


  **Configura el Backend:**
    ```sh
    cd backend
    # Crea y activa un entorno virtual
    python -m venv venv
    source venv/bin/activate # En Windows: venv\Scripts\activate
    # Instala las dependencias
    pip install -r requirements.txt
    ```


tu-proyecto-final/
├── .gitignore
├── README.md
├── frontend/           # Tu aplicación de React con Vite
│   ├── public/
│   ├── src/
│   │   ├── api/          # Lógica para conectar con el backend (Fetch)
│   │   ├── components/   # Componentes reutilizables (botones, navbars, etc.)
│   │   ├── pages/        # Vistas principales (Home, Login, Profile)
│   │   ├── styles/       # Archivos CSS o de estilos
│   │   └── main.jsx
│   ├── index.html
│   └── package.json
│
└── backend/            # Tu API de Flask
    ├── migrations/     # Archivos de migración de la base de datos
    ├── src/
    │   ├── api/          # Lógica de los endpoints de la API
    │   ├── models.py     # Definiciones de las tablas (SQLAlchemy)
    │   ├── app.py        # Archivo principal de la aplicación Flask
    │   ├── admin.py      # Configuración del panel de administrador (si aplica)
    │   └── utils.py      # Funciones de utilidad
    ├── .env            # Variables de entorno (claves de API, conexión a DB)
    ├── requirements.txt# Lista de dependencias de Python
    └── Pipfile         # Opcional, para gestión con pipenv
