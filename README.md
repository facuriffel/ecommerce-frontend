# Ecommerce Frontend

Frontend de una aplicación de ecommerce desarrollada con **Angular 18** y **PrimeNG 18**.

---

## 🛠️ Requisitos previos

Asegurate de tener instaladas las siguientes versiones:

| Herramienta | Versión requerida |
|-------------|-------------------|
| Node.js     | v22.x (LTS)       |
| Angular CLI | v18.2.x           |

> Podés verificar tu versión de Node con `node --version` y la de Angular CLI con `ng version`.

Para instalar Angular CLI globalmente (si no lo tenés):

```bash
npm install -g @angular/cli@18
```

---

## 📦 Instalación

Cloná el repositorio e instalá las dependencias:

```bash
git clone https://github.com/MaxiReichert/ecommerce-frontend.git
cd ecommerce-frontend
npm install
```

---

## 🚀 Levantar el proyecto

### Servidor de desarrollo

```bash
ng serve
```

La aplicación estará disponible en **http://localhost:4200/ecommerce/**.  
Se recarga automáticamente al detectar cambios en los archivos fuente.

> El `base href` está configurado como `/ecommerce/` para coincidir con el despliegue en Apache (`htdocs/ecommerce`).  
> Si preferís navegar en `localhost:4200/` sin el prefijo durante el desarrollo, podés correr:
> ```bash
> ng serve --base-href /
> ```

---

## ⚙️ Environments

La URL base del backend se configura por environment en `src/environments/`.

| Comando | Environment | Base URL del backend |
|---|---|---|
| `ng serve` | `environment.local.ts` | `http://localhost:8080/api` |
| `ng serve --configuration dev` | `environment.dev.ts` | `http://localhost:8080/ecommerce-1.0.0/api` |
| `ng build` | `environment.ts` (prod) | Configurar en `environment.ts` |

Para hacer el build de producción:

```bash
ng build
```

El resultado queda en `dist/ecommerce-frontend/` listo para copiar a `htdocs/ecommerce` en XAMPP.

## 🧱 Stack tecnológico

- **Angular** 18.2
- **PrimeNG** 18.0
- **PrimeIcons** 7.0
- **RxJS** 7.8
- **TypeScript** 5.5
