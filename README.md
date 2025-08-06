# 💻 Digitalízame - Backend

Backend del sistema **Digitalízame**, desarrollado con **Spring Boot** bajo arquitectura **MVC**. Esta aplicación provee la API para gestionar datos que serán consumidos por el frontend hecho en HTML, CSS y JavaScript.

---

## 🧱 Estructura del proyecto (MVC)

digitalizame-backend/
├── src/
│ ├── main/
│ │ ├── java/
│ │ │ └── com/
│ │ │ └── digitalizame/
│ │ │ ├── DigitalizameBackendApplication.java # Main
│ │ │ ├── controller/ # Controladores REST (Capa Controller)
│ │ │ ├── model/ # Entidades (Capa Modelo)
│ │ │ ├── repository/ # Interfaces de persistencia JPA
│ │ │ └── service/ # Lógica de negocio (Capa Service)
│ │ └── resources/
│ │ ├── application.properties # Configuración del proyecto
│ │ └── static/ # Recursos estáticos (si aplica)
├── pom.xml
└── README.md


---

## ⚙️ Tecnologías utilizadas

| Componente   | Herramienta              |
|--------------|--------------------------|
| Lenguaje     | Java 17 / 21             |
| Framework    | Spring Boot              |
| Persistencia | Spring Data JPA          |
| Base de datos| MySQL                    |
| Pruebas BD   | H2 (en memoria, dev)     |
| Frontend     | HTML, CSS y JavaScript   |
| IDE sugerido | IntelliJ IDEA o VS Code  |
| Build Tool   | Maven                    |

---

## ⚙️ Configuración de base de datos (MySQL)

En el archivo `src/main/resources/application.properties`, configura:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/digitalizame
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
