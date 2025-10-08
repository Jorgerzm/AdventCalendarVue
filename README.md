# Advent Calendar Vue

Este proyecto es un calendario de adviento interactivo desarrollado con Vue.js. Cada día del calendario revela una sorpresa o contenido especial, ideal para celebraciones navideñas o eventos de cuenta regresiva.

## Características
- 24 días con contenido personalizado
- Navegación entre días y regreso al calendario principal
- Animaciones y recursos multimedia (videos, imágenes)
- Estructura modular con componentes reutilizables

## Estructura del Proyecto
```
├── public/
│   ├── favicon.ico
│   └── index.html
├── src/
│   ├── App.vue
│   ├── main.js
│   ├── assets/
│   │   ├── octagon.mp4
│   │   ├── particles.mp4
│   │   └── snowflakes.mp4
│   ├── components/
│   │   ├── BackToCalendar.vue
│   │   ├── Day.vue
│   │   └── days/
│   │       ├── Day01.vue ... Day24.vue
│   ├── router/
│   │   └── index.js
│   └── views/
│       └── Calendar.vue
├── package.json
├── vue.config.js
├── babel.config.js
└── docker-compose.yml
```

## Instalación
1. Clona el repositorio:
   ```sh
   git clone https://github.com/Jorgerzm/AdventCalendarVue.git
   cd AdventCalendarVue
   ```
2. Instala las dependencias:
   ```sh
   npm install
   ```
3. Inicia el servidor de desarrollo:
   ```sh
   npm run serve
   ```
4. Abre tu navegador en `http://localhost:8080`

## Uso
- Haz clic en cualquier día disponible para ver el contenido especial.
- Usa el botón de regreso para volver al calendario principal.

## Personalización
- Modifica los archivos en `src/components/days/` para cambiar el contenido de cada día.
- Puedes agregar imágenes, videos o cualquier recurso multimedia en `src/assets/`.

## Tecnologías Utilizadas
- [Vue.js](https://vuejs.org/)
- JavaScript (ES6+)
- HTML5 y CSS3
