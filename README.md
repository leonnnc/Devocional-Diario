# 📖 Devocional Diario

Una aplicación web para el estudio bíblico diario con funcionalidades de lectura, planes de estudio y sistema de donaciones.

## 🚀 Funcionalidades Principales

### ✅ Completadas
- **📅 Devocional Diario**: Lectura diaria con versículos
- **📚 Lectura Bíblica**: Navegación por libros y capítulos
- **📋 Planes de Lectura**: Planes de 30, 60 y 90 días
- **🔍 Estudio Bíblico**: Búsqueda de versículos con notas personales
- **💰 Sistema de Donaciones**: Modal con QR de Yape y contacto email
- **📱 Exportación**: PDF y Word para WhatsApp
- **🎨 Diseño Responsive**: Optimizado para móvil y desktop

## 📁 Estructura del Proyecto

```
devocional-diario/          # Aplicación principal Next.js
├── src/
│   ├── components/         # Componentes React
│   │   ├── Navigation.tsx  # Navegación principal
│   │   ├── DonationModal.tsx # Modal de donaciones
│   │   ├── EstudioApp.tsx  # Sistema de estudio bíblico
│   │   ├── DevotionalApp.tsx # Devocional diario
│   │   ├── LecturaApp.tsx  # Sistema de lectura
│   │   ├── PlanApp.tsx     # Planes de lectura
│   │   └── ...
│   ├── utils/             # Utilidades y helpers
│   ├── data/              # Datos bíblicos en JSON
│   └── __tests__/         # Tests automatizados
├── public/                # Archivos estáticos
│   └── yape-qr.png       # QR de Yape real
└── ...

.kiro/                     # Configuración de Kiro
├── specs/                 # Especificaciones del proyecto
└── ...

docs/                      # Documentación técnica
├── ESTUDIO_IMPLEMENTATION.md
├── ADMIN_PANEL_IMPLEMENTATION.md
├── INLINE_BIBLE_TEXT_IMPLEMENTATION.md
├── PLAN_60_DAYS_CORRECTION.md
└── WHATSAPP_REMINDER_IMPLEMENTATION.md

scripts/                   # Scripts de conversión y utilidades
├── README.md              # Documentación de scripts
├── convert-all-books.py   # Conversión completa de la Biblia
├── convertir-libro.py     # Conversión de libros prioritarios
├── convert-bible-data.js  # Conversión JS completa
├── convert-single-book.js # Conversión individual JS
├── convert_genesis.py     # Conversión específica de Génesis
└── update_numruns.js      # Optimización de tests

backups/                   # Backups del proyecto
├── devocional-diario-backup-2026-01-09_23-26-05/
└── devocional-diario-backup-clean-2026-01-11_17-09-21/
```

## 🛠️ Tecnologías

- **Frontend**: Next.js 14, React, TypeScript
- **Styling**: CSS-in-JS (styled components inline)
- **Data**: JSON estático para datos bíblicos
- **Testing**: Jest, React Testing Library
- **Export**: jsPDF para PDFs, HTML para Word docs

## 🎯 Características del Sistema de Donaciones

- ⭐ Botón estrella dorado en navegación
- 📱 QR de Yape real integrado
- 📧 Email de contacto: devo.diaria@gmail.com
- 🎨 Modal elegante con tema oscuro
- 📱 Responsive design

## 🔍 Sistema de Estudio Bíblico

- 🔍 Búsqueda por referencia (ej: Juan 3:16)
- 📝 Notas personales por versículo
- 🏷️ Etiquetas AT/NT por testamento
- 📱 Exportación PDF y Word para WhatsApp
- 💾 Persistencia en localStorage
- 🎨 Autocompletado de libros bíblicos

## 📋 Planes de Lectura

- 📅 Plan 30 días: Lectura básica
- 📅 Plan 60 días: Lectura intermedia  
- 📅 Plan 90 días: Lectura completa
- 📊 Seguimiento de progreso
- 👤 Sistema de usuarios

## 🔧 Scripts y Utilidades

El proyecto incluye scripts de conversión para datos bíblicos:

- **📚 Conversión de Datos**: Scripts Python y JavaScript para convertir datos RV1960 al formato de la aplicación
- **🛠️ Utilidades**: Scripts para optimización de tests y mantenimiento
- **📖 Documentación**: Ver `scripts/README.md` para detalles completos

### Scripts Principales
- `convert-all-books.py` - Conversión completa de los 66 libros bíblicos
- `convertir-libro.py` - Conversión de libros prioritarios para desarrollo
- `update_numruns.js` - Optimización de tiempo de ejecución de tests

## 🚀 Instalación y Desarrollo

```bash
cd devocional-diario
npm install
npm run dev
```

## 📞 Contacto

Para contribuciones o consultas: **devo.diaria@gmail.com**

## 📄 Licencia

Proyecto personal para crecimiento espiritual.

---

**Estado del Proyecto**: ✅ Funcional y listo para producción
**Última Actualización**: Enero 2026