# 🏆 Mundial 2026 Quiz — Amalga Group

Juego de trivia multijugador con temática del Mundial FIFA 2026 para Team Wide Call.

## Estructura

```
mundial-quiz/
├── index.html      ← App completa (single file)
├── vercel.json     ← Config para deploy en Vercel
├── .gitignore
└── README.md
```

## Cómo usar

### Como HOST
1. Abre `index.html` en el navegador
2. Escribe un Room ID (ej: `amalga2026`)
3. Click **Entrar como HOST**
4. Copia los links de cada equipo desde el panel y compártelos

### Como Jugador
Abre el link que te dio el host, elige tu país y entra.

## Formato del torneo
- **8 equipos** — México, Brasil, España, Argentina, Francia, Alemania, Portugal, Inglaterra
- **Bracket eliminatorio** — Cuartos → Semis → Gran Final
- **Gana el primero en llegar a 3 goles** por partido
- **74 preguntas** en el banco, opción múltiple A/B/C/D
- Música, confetti y efectos de sonido incluidos

## Deploy en Vercel
1. Sube esta carpeta a un repo de GitHub
2. Conecta el repo en vercel.com
3. Framework: `Other`, Build command: vacío, Output: vacío
4. Deploy ✓

## Nota sobre multiplayer
El juego usa `localStorage` + `BroadcastChannel` para sincronización.  
Funciona entre tabs del mismo navegador.  
Para multidispositivo real se requiere backend (Supabase Realtime).
