# 🚀 Instrucciones para Subir a GitHub

Esta guía te llevará paso a paso para subir **Devocional Diario** a GitHub y configurar todo correctamente.

## 📋 Prerrequisitos

- ✅ Cuenta de GitHub creada
- ✅ Git instalado en tu sistema
- ✅ Proyecto funcionando localmente

## 🔧 Paso 1: Preparar el Repositorio Local

```bash
# 1. Navegar al directorio del proyecto
cd devocional-diario

# 2. Inicializar Git (si no está inicializado)
git init

# 3. Agregar todos los archivos
git add .

# 4. Hacer el commit inicial
git commit -m "feat: initial commit - devocional diario v1.0.0

✨ Funcionalidades implementadas:
- Devocional diario con versículos RV1960
- Sistema de estudio bíblico con búsqueda
- Planes de lectura (30, 60, 90 días)
- Exportación PDF/Word para WhatsApp
- Sistema de donaciones con Yape
- Diseño responsive con tema oscuro
- Suite completa de tests
- Documentación completa

🛠️ Tecnologías:
- Next.js 14 + TypeScript
- React 18 + CSS-in-JS
- Jest + Property-Based Testing
- jsPDF + Vercel deployment ready"
```

## 🌐 Paso 2: Crear Repositorio en GitHub

### Opción A: Desde GitHub Web
1. Ve a [github.com](https://github.com)
2. Haz clic en **"New repository"** (botón verde)
3. Configura el repositorio:
   - **Repository name**: `devocional-diario`
   - **Description**: `📖 Aplicación web moderna para estudio bíblico diario con RV1960, planes de lectura y sistema de donaciones`
   - **Visibility**: Public (recomendado) o Private
   - **NO marques**: "Add a README file" (ya tenemos uno)
   - **NO marques**: "Add .gitignore" (ya tenemos uno)
   - **NO marques**: "Choose a license" (ya tenemos LICENSE)
4. Haz clic en **"Create repository"**

### Opción B: Desde GitHub CLI (si tienes gh instalado)
```bash
gh repo create devocional-diario --public --description "📖 Aplicación web moderna para estudio bíblico diario con RV1960, planes de lectura y sistema de donaciones"
```

## 🔗 Paso 3: Conectar y Subir

```bash
# 1. Agregar el remote de GitHub
git remote add origin https://github.com/TU-USUARIO/devocional-diario.git

# 2. Verificar que el remote se agregó correctamente
git remote -v

# 3. Cambiar a la rama main (si no estás ya)
git branch -M main

# 4. Subir el código por primera vez
git push -u origin main
```

## ⚙️ Paso 4: Configurar GitHub (Opcional pero Recomendado)

### 4.1 Configurar Branch Protection
1. Ve a tu repositorio en GitHub
2. **Settings** → **Branches**
3. **Add rule** para la rama `main`:
   - ✅ Require pull request reviews before merging
   - ✅ Require status checks to pass before merging
   - ✅ Require branches to be up to date before merging
   - ✅ Include administrators

### 4.2 Configurar GitHub Actions Secrets (para CI/CD)
1. Ve a **Settings** → **Secrets and variables** → **Actions**
2. Agregar estos secrets (opcionales para deployment):
   ```
   VERCEL_TOKEN=tu_token_de_vercel
   ORG_ID=tu_org_id_de_vercel
   PROJECT_ID=tu_project_id_de_vercel
   CODECOV_TOKEN=tu_token_de_codecov (opcional)
   SNYK_TOKEN=tu_token_de_snyk (opcional)
   ```

### 4.3 Configurar Topics y About
1. En la página principal del repo, haz clic en ⚙️ junto a "About"
2. **Description**: `📖 Aplicación web moderna para estudio bíblico diario con RV1960, planes de lectura y sistema de donaciones`
3. **Website**: `https://tu-dominio.vercel.app` (cuando tengas el deploy)
4. **Topics**: `nextjs`, `react`, `typescript`, `bible`, `devotional`, `spanish`, `rv1960`, `study`, `prayer`, `christian`

## 🚀 Paso 5: Deploy en Vercel

### 5.1 Conectar con Vercel
1. Ve a [vercel.com](https://vercel.com)
2. **Sign up** con tu cuenta de GitHub
3. **Import Project** → selecciona tu repositorio `devocional-diario`
4. **Deploy** (Vercel detectará automáticamente que es Next.js)

### 5.2 Configurar Dominio (Opcional)
```bash
# Si tienes Vercel CLI instalado
vercel domains add tu-dominio.com
```

## 📊 Paso 6: Configurar Badges en README

Una vez que tengas el repositorio público, actualiza los badges en el README:

```markdown
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/TU-USUARIO/devocional-diario)
[![GitHub stars](https://img.shields.io/github/stars/TU-USUARIO/devocional-diario?style=social)](https://github.com/TU-USUARIO/devocional-diario/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/TU-USUARIO/devocional-diario?style=social)](https://github.com/TU-USUARIO/devocional-diario/network/members)
[![GitHub issues](https://img.shields.io/github/issues/TU-USUARIO/devocional-diario)](https://github.com/TU-USUARIO/devocional-diario/issues)
[![GitHub license](https://img.shields.io/github/license/TU-USUARIO/devocional-diario)](https://github.com/TU-USUARIO/devocional-diario/blob/main/LICENSE)
```

## 🔄 Paso 7: Workflow de Desarrollo Futuro

### Para cambios futuros:
```bash
# 1. Crear nueva rama para feature
git checkout -b feature/nueva-funcionalidad

# 2. Hacer cambios y commits
git add .
git commit -m "feat: agregar nueva funcionalidad"

# 3. Subir la rama
git push origin feature/nueva-funcionalidad

# 4. Crear Pull Request en GitHub
# 5. Después del merge, actualizar main local
git checkout main
git pull origin main
```

## 📱 Paso 8: Compartir el Proyecto

### URLs importantes:
- **Repositorio**: `https://github.com/TU-USUARIO/devocional-diario`
- **Demo en vivo**: `https://tu-proyecto.vercel.app`
- **Documentación**: El README.md se mostrará automáticamente

### Para promocionar:
1. **Compartir en redes sociales**
2. **Agregar a tu portafolio**
3. **Enviar a comunidades cristianas de desarrollo**
4. **Considerar enviar a showcases de Next.js**

## 🛡️ Paso 9: Seguridad y Mantenimiento

### Configurar Dependabot (automático en GitHub)
1. Ve a **Settings** → **Security & analysis**
2. Habilita **Dependabot alerts** y **Dependabot security updates**

### Configurar Code Scanning
1. Ve a **Security** → **Code scanning**
2. **Set up CodeQL analysis**

## 📞 Soporte

Si tienes problemas:

1. **GitHub Issues**: Usa las plantillas incluidas
2. **GitHub Discussions**: Para preguntas generales
3. **Email**: devo.diaria@gmail.com

## ✅ Checklist Final

- [ ] Repositorio creado en GitHub
- [ ] Código subido correctamente
- [ ] README.md se ve bien en GitHub
- [ ] GitHub Actions funcionando (si configuraste CI/CD)
- [ ] Deploy en Vercel exitoso
- [ ] Dominio configurado (opcional)
- [ ] Badges actualizados
- [ ] Topics y descripción configurados
- [ ] Branch protection habilitado
- [ ] Dependabot habilitado

## 🎉 ¡Felicidades!

Tu proyecto **Devocional Diario** está ahora:
- ✅ En GitHub con documentación completa
- ✅ Desplegado en Vercel
- ✅ Listo para recibir contribuciones
- ✅ Preparado para crecer y evolucionar

---

**¡Tu aplicación de estudio bíblico está lista para bendecir a miles de personas! 🙏**