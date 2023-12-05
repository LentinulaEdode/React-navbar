Este código es parte de una barra de navegación (Navbar) en una aplicación React que utiliza React Router.

En React, los hooks son funciones especiales que permiten a los componentes de función acceder al estado y a otras características de React. Estas funciones se llaman "hooks" porque permiten "engancharse" al ciclo de vida de los componentes y a otras características de React.

Los Hooks empleados para esto, son los siguientes: 

- useResolvedPath: Esta función toma una ruta y resuelve todas las variables y comodines en la ruta. Devuelve un objeto con las propiedades pathname, search, y hash. Esto es útil para garantizar que las rutas y los enlaces se resuelvan correctamente, incluso si tienen comodines o variables.

- useMatch: Esta función verifica si la ruta actual coincide con la ruta proporcionada. Puedes proporcionar opciones adicionales para ajustar el comportamiento de coincidencia. En este caso, se está utilizando con {path: resolvedPath.pathname, end: true} para verificar si la ruta actual coincide exactamente con la ruta proporcionada y no es parte de una coincidencia más larga.

En el componente CustomLink, estas funciones se utilizan para determinar si el enlace actual es activo. Si es así, se agrega la clase "active" al elemento <li>. Se sombreará de un colorín bonito.

En resumen, useResolvedPath se utiliza para resolver la ruta y useMatch se utiliza para verificar si la ruta actual coincide con la ruta proporcionada.

Próximamente, la barra de navegación pretende estar activa para construir un portfolio de presentación como junior entrépida. 


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

