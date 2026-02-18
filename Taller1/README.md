# Taller 1: CI/CD Pipeline con Express y GitHub Actions

## 📋 Descripción

API REST con pipeline automatizado de CI/CD usando Express, Jest y GitHub Actions.

---

## 🚀 Endpoints

- **GET `/`** → `{ "message": "Hola, DevOps!" }`
- **GET `/health`** → `{ "status": "OK", "timestamp": "..." }`
- **GET `/version`** → `{ "version": "1.0.0" }`

---

## 📁 Estructura

```
Taller1/
├── src/app.js                    # API Express
├── tests/app.test.js             # Tests unitarios
├── .github/workflows/ci.yml       # Pipeline CI/CD
└── package.json
```

---

## ⚡ Instalación y Uso

**Instalar:**
```bash
npm install
```

**Ejecutar servidor:**
```bash
npm start
```

**Correr tests:**
```bash
npm test
```

---

## 🧪 Tests

El proyecto incluye 3 tests unitarios (todos pasan ✅):

```bash
PASS tests/app.test.js
  ✓ GET / should return welcome message
  ✓ GET /health should return OK status
  ✓ GET /version should return version

Tests: 3 passed, 3 total
Coverage: 76.92%
```

---

## 🔄 Pipeline CI/CD

El workflow se ejecuta automáticamente en cada push:

1. **test** - Ejecuta tests con Jest
2. **build** - Verifica compilación
3. **deploy** - Publica en GitHub Pages (solo en `main`)

---

## 📊 GitHub Pages

Para habilitar despliegue automático:

1. Settings → Pages
2. Source: "Deploy from a branch"
3. Rama: `gh-pages`

Página: `https://uningenier0.github.io/Git-push-sin-miedo/`

---

**Profesor**: Sergio Vargas Parada | sevargasp@unal.edu.co

---

