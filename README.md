Pokémon Battle Game
Un juego de batalla Pokémon minimalista y retro construido con Next.js 15, TypeScript y CSS Modules. Selecciona dos Pokémon y observa épicas batallas con mecánicas basadas en estadísticas reales.

Pokémon Battle GameTypeScriptCSS Modules

Características
Interfaz Minimalista: Diseño limpio y funcional inspirado en juegos retro
Sistema de Batalla: Mecánicas basadas en estadísticas reales de Pokémon
Estadísticas de Juego: Seguimiento de batallas y ranking de ganadores
Tipos de Pokémon: Colores distintivos para cada tipo
Responsive Design: Optimizado para desktop, tablet y móvil
Performance: Carga rápida con optimizaciones de Next.js
Accesible: Diseño inclusivo con buenas prácticas de accesibilidad
Cómo Jugar
Cargar Pokémon: Haz clic en "Nuevos Pokémon" para obtener 12 Pokémon aleatorios
Seleccionar: Haz clic en 2 Pokémon para seleccionarlos (se resaltarán en amarillo)
Batalla Automática: La batalla comenzará automáticamente con animaciones
Ver Resultado: El ganador se determinará por estadísticas + factor suerte
Estadísticas: Revisa tus stats y el ranking de Pokémon ganadores
Tecnologías Utilizadas
Framework: Next.js 15 con App Router
Lenguaje: TypeScript
Estilos: CSS Modules para estilos encapsulados
API: PokéAPI para datos de Pokémon
Fuentes: Google Fonts (Press Start 2P)
Optimización: Next.js Image Optimization
 Instalación y Configuración
Prerrequisitos
Node.js 18.0 o superior
npm, yarn, pnpm o bun
Instalación
Clonar el repositorio
git clone https://github.com/tu-usuario/pokemon-battle-game.git
cd pokemon-battle-game
Instalar dependencias
npm install
# o
yarn install
# o
pnpm install
Ejecutar en desarrollo
npm run dev
# o
yarn dev
# o
pnpm dev
Abrir en el navegador
http://localhost:3000
Scripts Disponibles
npm run dev          # Ejecutar en modo desarrollo
npm run build        # Construir para producción
npm run start        # Ejecutar build de producción
npm run lint         # Ejecutar ESLint
npm run type-check   # Verificar tipos de TypeScript
 Estructura del Proyecto
pokemon-battle-game/
├── app/
│   ├── globals.css          # Estilos globales
│   ├── layout.tsx           # Layout principal
│   ├── page.tsx             # Página principal
│   └── page.module.css      # Estilos de la página principal
├── components/
│   ├── pokemon-card.tsx     # Componente de tarjeta Pokémon
│   ├── pokemon-card.module.css
│   ├── battle-arena.tsx     # Arena de batalla
│   ├── battle-arena.module.css
│   ├── game-stats.tsx       # Modal de estadísticas
│   └── game-stats.module.css
├── public/
│   └── placeholder.svg      # Imagen placeholder
├── README.md
├── next.config.js
├── package.json
└── tsconfig.json
 Componentes Principales
PokemonCard
Tarjeta individual de Pokémon con:

Imagen del Pokémon
Nombre e ID
Tipos con colores distintivos
Estadísticas básicas (HP, ATK)
Estados de selección y hover
BattleArena
Arena de batalla que muestra:

Dos Pokémon enfrentándose
Animaciones de batalla
Resultado del combate
Estados de ganador/perdedor
GameStats
Modal de estadísticas con:

Contador de batallas totales
Top 5 Pokémon ganadores
Opción para reiniciar estadísticas
🎨 Sistema de Tipos
El juego incluye colores distintivos para todos los tipos de Pokémon:

Tipo	Color
🔥 Fire	Rojo (#ff6b6b)
💧 Water	Azul (#4ecdc4)
🌱 Grass	Verde (#95e1d3)
⚡ Electric	Amarillo (#fce38a)
🔮 Psychic	Rosa (#f093fb)
❄️ Ice	Azul claro (#74b9ff)
🐉 Dragon	Púrpura (#6c5ce7)
🌙 Dark	Gris oscuro (#2d3436)
 Mecánicas de Batalla
La batalla se determina por:

Estadística de Ataque: Base stat del Pokémon
Experiencia Base: Influye en el poder total
Factor Suerte: Elemento aleatorio (0-50 puntos)
Fórmula: Poder = Ataque + (Experiencia/10) + Suerte

El Pokémon con mayor poder total gana la batalla.

📱 Responsive Design
Desktop: Grid de hasta 5 columnas
Tablet: Grid de 3-4 columnas
Móvil: Grid de 2 columnas
Controles: Se adaptan al tamaño de pantalla
🔧 Configuración Avanzada
Variables de Entorno
Crea un archivo .env.local para configuraciones personalizadas:

# Opcional: URL personalizada de la API
NEXT_PUBLIC_POKEMON_API_URL=https://pokeapi.co/api/v2
Personalización de Estilos
Los estilos están organizados en CSS Modules. Para personalizar:

Modifica los archivos .module.css correspondientes
Ajusta las variables CSS en globals.css
Cambia la fuente en layout.tsx

Fork el proyecto
Crea una rama para tu feature (git checkout -b feature/AmazingFeature)
Commit tus cambios (git commit -m 'Add some AmazingFeature')
Push a la rama (git push origin feature/AmazingFeature)
Abre un Pull Request
Guías de Contribución
Usa TypeScript para nuevos componentes
Sigue las convenciones de naming existentes
Añade CSS Modules para estilos
Incluye comentarios para lógica compleja
Mantén la accesibilidad en mente
Reportar Bugs
Si encuentras un bug, por favor:

Verifica que no esté ya reportado en Issues
Crea un nuevo issue con:
Descripción clara del problema
Pasos para reproducir
Comportamiento esperado vs actual
Screenshots si es relevante
