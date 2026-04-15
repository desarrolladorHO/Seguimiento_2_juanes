# RIHO Enterprise - Sistema de Gestión TI

![Status](https://img.shields.io/badge/Status-Producci%C3%B3n-38debb?style=for-the-badge)
![PHP](https://img.shields.io/badge/PHP-8.2-777bb4?style=for-the-badge&logo=php)
![SQL Server](https://img.shields.io/badge/SQL_Server-2019-CC2927?style=for-the-badge&logo=microsoft-sql-server)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-3.0-38B2AC?style=for-the-badge&logo=tailwind-css)

**RIHO** es un ecosistema técnico integral desarrollado para **Hernán Ocazionez Y CIA SAS**, diseñado para centralizar la gestión de soporte técnico, administración de credenciales y monitoreo de infraestructura en un entorno de IPS.

---

## 🚀 Componentes del Proyecto

El repositorio está estructurado en dos grandes bloques:

1.  **Landing Page Profesional**: Interfaz de alto impacto visual que sirve como portal de entrada y presentación del proyecto ante stakeholders.
2.  **Módulo Administrativo (Core)**: Aplicación funcional que interactúa con la base de datos para la gestión operativa diaria.

---

## 🛠️ Arquitectura Técnica

### Infraestructura de Datos
* **Engine:** Microsoft SQL Server.
* **Conectividad:** Driver nativo `sqlsrv` para PHP, optimizado para entornos Windows Server.
* **Estructura:** Uso de procedimientos almacenados y vistas para la generación de reportes y dashboards de rendimiento.

### Stack de Desarrollo
* **Backend:** PHP 8.2 (Estructura modular).
* **Frontend:** HTML5, Tailwind CSS y JavaScript.
* **Librerías de Visualización:** Chart.js para el análisis de métricas en el *Dashboard Proteo*.
* **Animaciones:** AOS (Animate On Scroll) para una experiencia de usuario fluida.

---

## 📦 Módulos del Sistema (RIHO Core)

Basado en la estructura de archivos operativa, el sistema cuenta con los siguientes módulos clave:

### 1. Gestión de Credenciales
Administración centralizada de accesos institucionales:
* `creden_actualizar.php`: Interfaz para modificación de parámetros de acceso.
* `creden_procesar_tipo.php`: Motor de lógica para la categorización de nuevas cuentas.
* `creden_inactivar_tipo.php`: Control de seguridad y auditoría de accesos.

### 2. Administración Operativa por Sedes
Gestión jerárquica de la infraestructura física:
* `areas_sistemas.php` & `categorias_sistemas.php`: Parametrización de la red institucional.
* `inicio_sede_sistemas.php`: Panel de control específico para la gestión técnica por ubicación.

### 3. Seguimiento TI
Módulo de respuesta técnica para incidentes:
* `agregar_seguimiento.php`: Registro detallado de acciones correctivas y preventivas.
* `consultar_estado.php`: Trazabilidad en tiempo real de los requerimientos de soporte.

---

## 🎨 Identidad Visual: RIHO

El proyecto introduce a **RIHO**, la mascota y asistente virtual del equipo de sistemas. Su presencia en la interfaz simboliza la automatización y el acompañamiento constante al usuario final dentro de la IPS.

> **Nota:** La landing page utiliza técnicas avanzadas de filtros CSS (`mix-blend-mode: screen`) para integrar a RIHO de forma nativa en el diseño Dark Mode, eliminando artefactos visuales y fondos no deseados.

---

## 👥 Equipo de Desarrollo

| Desarrollador | Especialidad | Rol en el Proyecto |
| :--- | :--- | :--- |
| **Juan Esteban Ospina Zapata** | Técnico en Análisis y Desarrollo de Software | Arquitectura de Base de Datos, Conectividad SQLSRV y Lógica Backend. |
| **Jeronimo Mesa Carvajal** | Software Development Engineer | Diseño de Interfaces, Gestión de Módulos Administrativos y UX. |

---

## ⚙️ Configuración del Entorno

1.  **Prerrequisitos:**
    * Servidor Web (Apache/IIS) con PHP 8.1+.
    * Extensiones `php_sqlsrv` y `php_pdo_sqlsrv` habilitadas.
    * Instancia de SQL Server con autenticación configurada.

2.  **Instalación:**
    ```bash
    git clone [https://github.com/desarrolladorHO/RIHO-Enterprise.git](https://github.com/desarrolladorHO/RIHO-Enterprise.git)
    ```

3.  **Base de Datos:**
    * Ejecutar los scripts de creación de tablas ubicados en la carpeta `/database`.
    * Configurar las variables de entorno en el archivo de conexión principal.

---

## 📄 Propiedad Intelectual
Este software ha sido desarrollado específicamente para **Hernán Ocazionez Y CIA SAS**. Queda prohibida su reproducción o distribución sin autorización expresa de los autores.

**© 2026 RIHO Enterprise Team**
