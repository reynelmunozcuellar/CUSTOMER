# CUSTOMER
Aplicación Android profesional para la gestión integral de negocios, diseñada para pequeños, medianos y grandes comercios.

## 🚀 Características Implementadas

### Base de Datos y Arquitectura
- ✅ Base de datos Room completa con todas las entidades necesarias
- ✅ DAOs y Repositorios implementados para todas las entidades
- ✅ Arquitectura MVVM con ViewModels y LiveData
- ✅ Sistema de preferencias para gestión de sesión

### Gestión Multi-Empresa
- ✅ Soporte para múltiples empresas en una sola aplicación
- ✅ Pantalla de selección y creación de empresas
- ✅ Aislamiento de datos por empresa

### Autenticación y Roles
- ✅ Sistema de login con usuarios
- ✅ Roles: Administrador y Vendedor
- ✅ Creación automática de usuario admin por defecto

### Gestión de Clientes
- ✅ CRUD completo de clientes
- ✅ Campos: nombre, teléfono, dirección, barrio, email
- ✅ Búsqueda de clientes por nombre o teléfono

### Gestión de Productos
- ✅ CRUD completo de productos
- ✅ Campos: código, nombre, descripción, precio, cantidad (stock), stop (stock mínimo)
- ✅ Soporte para múltiples imágenes por producto (hasta 3)
- ✅ Generación de códigos QR para productos
- ✅ Búsqueda de productos por código, nombre o descripción
- ✅ Gestión de stock crítico

### Sistema de Ventas
- ✅ Carrito de compras funcional
- ✅ Selección de cliente para ventas
- ✅ Registro de ventas con items
- ✅ Generación automática de número de factura
- ✅ Reducción automática de stock al vender

### Facturación PDF
- ✅ Generación profesional de facturas en PDF
- ✅ Formatos: Carta y Media Carta
- ✅ Orientación: Vertical y Horizontal
- ✅ Campos completos: empresa, cliente, items, totales, forma de pago
- ✅ Logo de empresa en facturas
- ✅ Tabla detallada de items con imágenes

### Compartir por WhatsApp
- ✅ Compartir facturas PDF por WhatsApp Business
- ✅ Mensajes personalizados automáticos
- ✅ Integración con WhatsApp Web

### Dashboard
- ✅ Vista general de ventas del día
- ✅ Vista de ventas del mes
- ✅ Espacio para gráficas de productos más vendidos (estructura lista)

### Interfaz de Usuario
- ✅ Material Design moderno
- ✅ Navegación por pestañas (Tabs)
- ✅ ViewPager2 para navegación fluida
- ✅ CardViews y componentes Material

## 📋 Características Pendientes de Implementar

### Funcionalidades Avanzadas
- ⏳ Catálogo de productos interactivo (pantalla completa)
- ⏳ Vista de catálogo vertical (1 imagen) y horizontal (3 imágenes)
- ⏳ Modo Kiosco para tablets
- ⏳ Escáner de códigos QR/barras con cámara
- ⏳ Búsqueda global inteligente (clientes, productos, facturas)

### Funcionalidades de Catálogo
- ⏳ Generación de catálogo en PDF
- ⏳ Compartir catálogo PDF por WhatsApp
- ⏳ Enlace web temporal para catálogo interactivo

### Gestión Avanzada
- ⏳ Edición completa de clientes y productos (pantallas de edición)
- ⏳ Subida de logos de empresa desde galería
- ⏳ Personalización de colores de la interfaz por empresa
- ⏳ Historial de precios de productos
- ⏳ Historial de compras por cliente (CRM)

### Dashboard y Reportes
- ⏳ Gráficas completas de productos más vendidos
- ⏳ Estadísticas por vendedor
- ⏳ Reportes consolidados multi-empresa
- ⏳ Cierre de caja diario

### Modo Offline
- ⏳ Sincronización automática al recuperar conexión
- ⏳ Indicador de estado de sincronización
- ⏳ Gestión de colas de sincronización

### Notificaciones
- ⏳ Notificaciones push para stock crítico
- ⏳ Alertas de productos con stock bajo

### Optimizaciones
- ⏳ Navegación por gestos (swipes) en catálogo
- ⏳ Búsqueda predictiva
- ⏳ Caché de imágenes
- ⏳ Optimización para tablets

## 🛠️ Tecnologías Utilizadas

- **Kotlin** - Lenguaje de programación
- **Android Architecture Components**:
  - Room Database
  - ViewModel & LiveData
  - ViewBinding
- **Material Design Components**
- **Coroutines** - Programación asíncrona
- **Glide** - Carga de imágenes
- **ZXing** - Generación y lectura de códigos QR
- **iText7** - Generación de PDFs
- **WorkManager** - Tareas en segundo plano

## 📦 Estructura del Proyecto

```
app/
├── data/
│   ├── database/
│   │   ├── entity/        # Entidades Room
│   │   ├── dao/           # Data Access Objects
│   │   └── AppDatabase.kt
│   ├── repository/        # Repositorios
│   ├── model/            # Modelos de datos
│   └── preferences/      # Gestión de preferencias
├── ui/
│   ├── splash/           # Selección de empresa y login
│   ├── dashboard/        # Dashboard principal
│   ├── ventas/           # Gestión de ventas
│   ├── productos/        # Gestión de productos
│   ├── clientes/         # Gestión de clientes
│   └── viewmodel/        # ViewModels
├── util/
│   ├── PdfUtil.kt        # Generación de PDFs
│   └── ShareUtil.kt      # Compartir por WhatsApp
└── work/                 # Workers (WorkManager)
```

## 🔧 Configuración

1. Clonar o descargar el proyecto
2. Abrir en Android Studio
3. Sincronizar Gradle
4. Ejecutar en dispositivo o emulador (API 26+)

## 📝 Notas Importantes

- La aplicación requiere permisos de cámara, almacenamiento e internet
- La primera vez que se inicia, se debe crear una empresa
- Se crea automáticamente un usuario admin con email: `admin@empresa.com` y contraseña: `admin123`
- Los PDFs se guardan en el almacenamiento interno de la aplicación

## 🎯 Próximos Pasos

1. Implementar pantallas completas de gestión (CRUD visual)
2. Agregar funcionalidad de cámara para QR/barras
3. Implementar catálogo interactivo completo
4. Agregar gráficas y reportes visuales
5. Implementar sincronización offline
6. Agregar notificaciones push

## 📄 Licencia

Este proyecto es de código abierto y está disponible para uso comercial y personal.

---

**Versión**: 1.0  
**Última actualización**: 2024
