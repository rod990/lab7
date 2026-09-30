# Catálogo de Servicios Web

> Aplicación web full-stack para la exposición y gestión de un catálogo de servicios mediante una API REST.

## 1. Descripción del proyecto
- **Problema o necesidad**: Centralizar el listado de servicios en una plataforma web única.
- **Usuarios objetivo**: Clientes finales y administradores del negocio.
- **Funcionalidades previstas**: CRUD de servicios y carrito de cotización.
- **Funcionalidades ya implementadas**: Diseño de base de datos relacional, modelo de Servicios, panel de administración básico en Django.

## 2. Equipo
| Integrante | Rol | Usuario GitHub |
|---|---|---|
| Rodolfo Aaron Durán Aravena | Backend / Frontend / Documentos | @rod9999 |

## 3. Stack y versiones
| Tecnología | Versión |
|---|---|
| Python | 3.12.x |
| Django | 5.0.x |
| Node.js / npm | 20.x LTS |
| React / Vite | React 18.x / Vite 5.x |
| Base de datos | SQLite3 |

## 4. Arquitectura
**Flujo**: Navegador -> React (Puerto 5173) -> (Proxy Vite) -> Django (Puerto 8000) -> SQLite.
**Estrategia elegida**: Aplicaciones independientes conectadas por API REST con proxy de Vite en desarrollo para evitar errores de CORS.

## 5. Estructura del repositorio
```text
/
├── backend/            # Proyecto Django 
├── frontend/           # Proyecto React 
├── docs/img/           # Capturas de evidencia del sistema
├── .gitignore          # Archivos excluidos de Git
└── README.md           # Documentación principal