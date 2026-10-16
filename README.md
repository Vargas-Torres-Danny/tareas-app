# ✅ App de Tareas — React + Node.js

Aplicación full-stack: frontend en **React (Vite)** y API REST en **Node.js + Express**.

## 🌐 URLs en vivo
- **Frontend (Vercel):** https://TU-APP.vercel.app
- **API (Render):** https://TU-API.onrender.com/api/tareas

> La API está en el plan gratuito de Render: si lleva 15 min sin uso, la primera petición tarda ~1 min en despertar.

## 📸 Capturas
![Render](capturas/render.png)
![Vercel](capturas/vercel.png)
![App en vivo](capturas/app.png)

## 🧱 Estructura
```
tareas-app/
├── server/   # Backend Node + Express
└── client/   # Frontend React + Vite
```

## ▶️ Ejecutar en local
```bash
# Terminal 1 - Backend
cd server && npm install && npm run dev      # http://localhost:3001

# Terminal 2 - Frontend
cd client && npm install && npm run dev      # http://localhost:5173
```

## 🔌 Endpoints
| Método | Ruta | Descripción |
|--------|------|-------------|
| GET | /api/tareas | Obtener todas las tareas |
| POST | /api/tareas | Crear una tarea |
| PUT | /api/tareas/:id | Completar/descompletar |
| DELETE | /api/tareas/:id | Eliminar una tarea |

## ⚙️ Variables de entorno
| Dónde | Variable | Valor |
|-------|----------|-------|
| Render (server) | `CLIENTE_URL` | URL del frontend en Vercel (sin `/` final) |
| Vercel (client) | `VITE_API_URL` | `https://TU-API.onrender.com/api/tareas` |

## 🚀 Despliegue
- **Backend:** Render → Root Directory `server`, Build `npm install`, Start `node index.js`.
- **Frontend:** Vercel → Root Directory `client`, Build `npm run build`, Output `dist`.
- Cada `git push` a `main` redespliega automáticamente.

## 🛠️ Tecnologías
React 18 · Vite · Node.js · Express · CORS · GitHub · Render · Vercel
