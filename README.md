# 🔐 AWS S3 Encryption & Logging Lab

Este laboratorio demuestra cómo implementar cifrado del lado del servidor (SSE) en un bucket S3 y habilitar el registro de accesos para auditoría. Es parte del aprendizaje de buenas prácticas de **seguridad en la nube (cloud security)**.

---

## 🧰 Servicios y herramientas utilizados

* **Amazon S3** — Almacenamiento de objetos y configuración de seguridad
* **AWS CLI** — Interacción mediante línea de comandos
* **IAM Policy** — Políticas para denegar accesos sin cifrado
* **Linux/WSL** — Entorno local de desarrollo
* **Git + GitHub** — Versionado y documentación del laboratorio

---

## 🧱 Estructura del proyecto

```plaintext
aws-s3-encryption-lab/
├── secure-bucket/              # Archivos de prueba para carga en el bucket
│   └── prueba.txt
├── iam/                        # Política IAM para exigir cifrado
│   └── policy.json
├── screenshots/                # Evidencia visual del laboratorio
│   └── (capturas del proceso)
└── README.md
```

---

## 🚀 Pasos realizados

1. Crear estructura del proyecto y repositorio local
2. Crear bucket con nombre dinámico desde CLI
3. Verificar cifrado por defecto
4. Crear una policy IAM que deniegue carga sin cifrado SSE
5. Cargar archivo correctamente cifrado (AES256)
6. Intentar cargar sin cifrado y observar bloqueo (AccessDenied)
7. Activar registros de acceso al bucket (logging)

---

## 📸 Evidencias del proceso

### 1️⃣ Estructura del proyecto creada

![01-estructura-proyecto](screenshots/01-estructura-proyecto.png)

### 2️⃣ Bucket creado con SSE habilitado

![02-bucket-creado-cifrado](screenshots/02-bucket-creado-cifrado.png)

### 3️⃣ Verificación del cifrado

![03-verificar-cifrado](screenshots/03-verificar-cifrado.png)

### 4️⃣ Política que bloquea carga sin cifrado SSE

![04-politica-bloqueo-sin-cifrado](screenshots/04-politica-bloqueo-sin-cifrado.png)

### 5️⃣ Carga permitida con cifrado SSE

![05-carga-bloqueada](screenshots/05-carga-bloqueada.png)

### 6️⃣ Activación del logging y configuración del destino

![06-activar-logs-config](screenshots/06-activar-logs-config.png)

### 7️⃣ Confirmación de logs habilitados correctamente

![07-logs-habilitados-confirmacion](screenshots/07-logs-habilitados-confirmacion.png)

---

## 🌍 Relevancia del laboratorio

Este ejercicio aplica conceptos esenciales de **seguridad en la nube**:

* Implementación de **cifrado obligatorio** (SSE)
* Prevención de errores por configuración incorrecta
* Auditoría mediante logs y detección de accesos

---

## 👤 Autor

**Sebastián Cárdenas**
*Aspirante a AWS Cloud Practitioner | Estudiante de Ingeniería en Ciberseguridad*
📫 Contacto: [sebastian.cardenas.t@gmail.com](mailto:sebastian.cardenas.t@gmail.com)

---

