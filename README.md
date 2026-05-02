# Template Lib GetX

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter&logoColor=white)
![GetX](https://img.shields.io/badge/GetX-State%20%7C%20Route%20%7C%20Dependency-0175C2)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

**Plantilla base para iniciar proyectos Flutter con arquitectura GetX de forma rápida y ordenada.**

</div>

---

## 🚀 ¿Qué incluye?

Este repositorio es un **scaffold / boilerplate** que te permite arrancar un proyecto Flutter profesional sin perder tiempo en la configuración inicial. Incluye la estructura de carpetas y los archivos base recomendados para trabajar con **GetX**.

### Estructura generada

```
lib/
├── main.dart                          # Punto de entrada con GetMaterialApp
├── core/
│   └── theme/
│       └── text_theme.dart            # Configuración tipográfica base
├── app/
│   ├── data/
│   │   ├── providers/                 # Fuente de datos (API, local, etc.)
│   │   └── services/                  # Lógica de negocio y casos de uso
│   ├── modules/
│   │   ├── home/                      # Módulo de inicio (View + Controller + Binding)
│   │   └── login/                     # Módulo de autenticación (View + Controller + Binding)
│   └── routes/
│       ├── app_pages.dart             # Definición de rutas y bindings
│       ├── app_routes.dart            # Constantes de rutas
│       └── middlewares/               # Middlewares (ej. guard de autenticación)
```

### Características incluidas

- ✅ **GetMaterialApp** configurado y listo
- ✅ **Routing** con `GetPage`, bindings y middlewares
- ✅ **AuthGuardMiddleware** de ejemplo para proteger rutas
- ✅ **Módulos de ejemplo** (`home`, `login`) con la separación View / Controller / Binding
- ✅ **Data layer** de ejemplo con providers y services
- ✅ **Tema tipográfico** base en `core/theme`

---

## 🛠️ Uso

### 1. Copiar la plantilla

Puedes copiar directamente los archivos de este repo en tu nuevo proyecto Flutter, o usarlo como referencia.

```bash
# Crear nuevo proyecto
flutter create mi_nuevo_proyecto
cd mi_nuevo_proyecto

# Copiar la estructura de este template al directorio lib/
```

### 2. Agregar dependencias

Asegúrate de incluir `get` en tu `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  get: ^4.6.6
```

```bash
flutter pub get
```

### 3. Ejecutar

```bash
flutter run
```

---

## 📦 Dependencias recomendadas (opcionales)

Según las necesidades de tu proyecto, puedes agregar:

| Paquete | Uso |
|---------|-----|
| `get` | Gestión de estado, rutas y dependencias (ya incluido) |
| `google_fonts` | Tipografías de Google |
| `http` / `dio` | Consumo de APIs REST |
| `hive` / `shared_preferences` | Almacenamiento local |
| `intl` | Internacionalización y formatos |

---

## 🤝 Contribución

Si tienes mejoras para esta plantilla (nuevos middlewares, módulos de ejemplo, configuraciones de tema, etc.), ¡los Pull Requests son bienvenidos!

---

## 📄 Licencia

Este proyecto está bajo la licencia **MIT**. Consulta el archivo [`LICENSE`](LICENSE) para más detalles.

---

<div align="center">

**⭐ Úsalo como base para tus proyectos Flutter + GetX ⭐**

</div>
