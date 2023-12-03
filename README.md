# Modulo_React

## ReactJS y sus principales características:
ReactJS es la salvación de muchos desarrolladores front-end jaja, es una biblioteca de JavaScript utilizada para construir interfaces de usuario interactivas. Sus características clave incluyen el enfoque en componentes reutilizables, el uso de un Virtual DOM para optimizar las actualizaciones de la interfaz, y la capacidad de unir datos unidireccionalmente, lo que mejora la predictibilidad y el rendimiento.

### Componentes en ReactJS:
Como de dijo en las caracteristicas claves, un componente en ReactJS es una pieza de la interfaz de usuario. Se dividen en dos tipos principales: componentes funcionales, basados en funciones de JavaScript, y componentes de clase, basados en clases ES6. Los componentes funcionales son más simples y modernos, mientras que los de clase tienen ciclos de vida más complejos.

### Virtual DOM en ReactJS:
Tambien como se dijo en las característiccas claves, el Virtual DOM es una representación ligera y virtual del DOM real. React utiliza el Virtual DOM para realizar comparaciones eficientes entre el estado actual y anterior de la interfaz de usuario. Esto minimiza las manipulaciones directas en el DOM, mejorando el rendimiento al actualizar solo las partes necesarias.

### JSX en ReactJS:
Y bueno, cual es la sintaxís principal de React? exacto es JSX, aunque realmente JSX es una extensión de sintaxis para JavaScript utilizada con React. Permite escribir código similar a HTML dentro de JavaScript, facilitando la creación de componentes de manera declarativa. JSX es importante porque simplifica la creación de interfaces de usuario en React y mejora la legibilidad del código.

## Hooks en ReactJS y su propósito:
Un Hook en ReactJS es una función especial que permite utilizar características de React en componentes funcionales. Su propósito es agregar estado, ciclo de vida y otras características de las clases a los componentes funcionales, mejorando la reutilización del código.

### Tipos de Hooks en ReactJS:
   - **useState:** Permite agregar estado a componentes funcionales.
   - **useEffect:** Gestiona efectos secundarios en componentes funcionales, como peticiones a API.
   - **useContext:** Facilita el consumo de contextos en componentes funcionales.

### Reglas de uso para los Hooks en ReactJS:
   - Solo se pueden usar en componentes funcionales o en custom Hooks.
   - Deben llamarse en el nivel superior del componente.
   - Deben ser llamados en el mismo orden en cada renderización.
   -
## React Router DOM versión 6:
Bueno, ya sabiendo como funciona las plantillas y sus estados, cómo podemos navegar?, con React Router DOM, es una biblioteca para el enrutamiento en aplicaciones React. La versión 6 presenta un modelo simplificado y utiliza Hooks. Sus componentes clave son `BrowserRouter` para envolver la aplicación, `Route` para definir rutas, y `useNavigate` para la navegación programática.

### Navegación con React Router DOM:
Para navegar entre páginas, se utiliza el hook `useNavigate` proporcionado por React Router DOM. Al hacer clic en un enlace o un botón, se llama a `useNavigate` con la ruta de destino. 
Por ejemplo:

   ```jsx
   import { useNavigate } from 'react-router-dom';

   // ...

   const navigate = useNavigate();

   // ...

   <button onClick={() => navigate('/ruta-destino')}>Ir a la Ruta</button>
   ```

Esto activa la navegación y renderiza el componente asociado a la nueva ruta, proporcionando una experiencia de navegación suave en la aplicación React.

- **Crear un proyecto ReactJS con Vite:**
   Para crear un proyecto ReactJS con Vite, sigue estos pasos:
   ```bash
   # Instalar Vite globalmente (solo la primera vez)
   npm install -g create-vite

   # Crear un proyecto React con Vite
   create-vite my-react-app --template react

   # Ir al directorio del proyecto
   cd my-react-app

   # Instalar dependencias
   npm install

   # Iniciar el servidor de desarrollo
   npm run dev
   ```
   Esto utiliza el generador `create-vite` para crear un proyecto React con Vite.

**Desplegar un JSON server:**
   Para desplegar un JSON server en un hosting gratuito o servicio en la nube:
   - Instala `json-server` globalmente: `npm install -g json-server`
   - Crea un archivo JSON con tus datos.
   - Ejecuta `json-server --watch tu-archivo-json.json` en tu máquina local.
   - Utiliza servicios como Heroku o Vercel para desplegar tu servidor JSON.

**Desplegar una aplicación React en cualquier hosting:**
   Desplegar una aplicación React en cualquier hosting implica:
   - Construir la aplicación: `npm run build`
   - Subir los archivos generados en la carpeta `build` a tu servicio de hosting.
   - Configurar el servidor web para servir estos archivos estáticos.
   - Ejemplos de hostings gratuitos incluyen Netlify, Vercel, GitHub Pages, y Firebase Hosting. Sube los archivos o conecta tu repositorio, y el servicio se encargará del despliegue.
