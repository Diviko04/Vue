# Proyecto Vue.js con Vite y Vue CLI

## Descripción
Este documento describe dos formas de crear un proyecto Vue.js: utilizando Vue CLI (opción tradicional) o Vite (opción recomendada). Se explican las ventajas y desventajas de cada método, así como la estructura de carpetas de un proyecto Vue.

## Instalación

### Opción tradicional: Vue CLI
Vue CLI es una herramienta más antigua para la creación de proyectos Vue. Aunque sigue siendo funcional, Vite es la opción recomendada en Vue 3.

#### Pasos de instalación
```sh
npm install -g @vue/cli
vue create my-project
cd my-project
npm run serve
```

#### Desventajas
- Vue CLI es menos eficiente en Vue 3.
- Su velocidad y optimización son inferiores a las de Vite.

### Opción recomendada: Vite
Vite es la herramienta más moderna y rápida para crear proyectos Vue, con mejor rendimiento y carga en caliente.

#### Pasos de instalación
```sh
npm create vite@latest vue-app --template vue
cd vue-app
npm install
npm run dev
```

#### Ventajas
- Carga rápida.
- Hot Module Replacement (HMR) para una mejor experiencia de desarrollo.
- Mejor optimización general.

#### Requisitos
- Es necesario tener Node.js instalado.

## Estructura del Proyecto

Una vez creado el proyecto, su estructura se verá de la siguiente manera:

```
vue-app/
│── node_modules/
│── public/
│── src/
│   │── assets/
│   │── components/
│   │── App.vue
│   │── main.js
│── index.html
│── package.json
│── vite.config.js
```

### Explicación de carpetas y archivos
- **`src/`** (Código fuente)
  - **`assets/`**: Almacena recursos estáticos como imágenes y estilos globales.
  - **`components/`**: Contiene componentes Vue reutilizables.
  - **`App.vue`**: Componente principal de la aplicación.
  - **`main.js`**: Punto de entrada donde se inicializa Vue.
- **`public/`** (Archivos estáticos)
  - Archivos que no se procesan en la compilación, como `favicon.ico`.
- **Otros archivos importantes**
  - **`node_modules/`**: Contiene las dependencias del proyecto (no se edita manualmente).
  - **`.gitignore`**: Define archivos y carpetas a excluir de Git.
  - **`package.json`**: Archivo de configuración del proyecto (dependencias y scripts).
  - **`vite.config.js`**: Configuración del servidor de desarrollo con Vite.
  - **`index.html`**: Archivo HTML principal donde se monta Vue.
  - **`package-lock.json`**: Bloquea las versiones exactas de las dependencias.

## Fundamentos de Vue.js
Vue.js se basa en componentes y reactividad, lo que permite:
- Inicializar la aplicación y conectarla al DOM.
- Definir la lógica de la app con variables, funciones y estados.
- Controlar la reactividad (actualización automática de la interfaz cuando los datos cambian).
- Gestionar componentes reutilizables.

## Conclusión
Vite es la herramienta recomendada para iniciar proyectos Vue.js en la actualidad, ofreciendo un entorno de desarrollo más rápido y eficiente en comparación con Vue CLI. Siguiendo esta guía, podrás configurar y comprender la estructura de un proyecto Vue de manera sencilla.

