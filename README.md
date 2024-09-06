# Proyecto Contador de Calorías - useReducer y Context API

Este proyecto es un contador de calorías donde los usuarios pueden ingresar alimentos o ejercicios con su nivel de calorías a través de un formulario, y la aplicación los lista permitiendo editarlos o eliminarlos. Además, calcula las calorías consumidas, las quemadas y la diferencia numérica entre estas para llevar un control de la alimentación.

Puedes ver la aplicación en acción [aquí](https://react-contador-calorias.netlify.app).

## Tabla de Contenidos

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Instalación](#instalación)
- [Funcionalidades](#funcionalidades)
- [Aprendizaje Clave: useReducer y Context API](#aprendizaje-clave-usereducer-y-context-api)
- [Créditos](#créditos)
- [Conclusión](#conclusión)

## Descripción del Proyecto

La aplicación permite a los usuarios ingresar alimentos o ejercicios con su nivel de calorías, listarlos, editarlos o eliminarlos. A su vez, la aplicación calcula:

- **Calorías consumidas**.
- **Calorías quemadas**.
- **Diferencia entre calorías consumidas y quemadas**.

Este proyecto ha sido migrado a **useReducer** para manejar el estado de los alimentos y ejercicios de manera más eficiente. Ahora también utiliza **Context API** para manejar el reducer de manera global, eliminando la necesidad de pasar el estado y las funciones de dispatch a través de props, lo que ha mejorado considerablemente la organización del código.

## Tecnologías Utilizadas

- **React**: Biblioteca para la creación de interfaces de usuario.
- **TypeScript**: Lenguaje con tipado estático.
- **Tailwind CSS**: Framework CSS para estilizar rápidamente la interfaz.
- **useReducer**: Hook utilizado para gestionar el estado de manera eficiente.
- **Context API**: API de React que permite manejar el estado de forma global.

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tuusuario/contador-calorias.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd contador-calorias
   ```
3. Instala las dependencias:
   ```bash
   npm install
   ```
4. Inicia el servidor de desarrollo:
   ```bash
   npm run dev
   ```

## Funcionalidades

- **Agregar Alimentos o Ejercicios**: A través de un formulario, los usuarios pueden añadir alimentos o ejercicios con sus calorías.
- **Editar o Eliminar Entradas**: Los usuarios pueden modificar o eliminar cualquier alimento o ejercicio registrado.
- **Cálculo Automático**: La aplicación calcula automáticamente las calorías consumidas, quemadas, y muestra la diferencia entre ambas.

## Aprendizaje Clave: useReducer y Migración a Context API

Anteriormente, el proyecto manejaba el estado de los alimentos y ejercicios usando `useReducer` pero pasaba el estado y las funciones de dispatch a través de props. Tras migrar a **Context API**, el manejo del estado ahora es global, lo que elimina la necesidad de pasar props innecesarias y simplifica la estructura de los componentes.

### Beneficios de Context API:

- **Manejo Global del Estado**: Context API permite acceder al estado y las funciones de dispatch en cualquier componente sin necesidad de pasar props, lo que hace el código más limpio y manejable.
- **Mejora en la Escalabilidad**: La migración a Context API facilita el crecimiento de la aplicación, ya que la gestión del estado está centralizada.

Esta migración fue fundamental para entender cómo organizar mejor las aplicaciones grandes y evitar el llamado "prop drilling" (el paso excesivo de props entre componentes).

## Créditos

Este proyecto fue desarrollado como parte del curso de React y TypeScript de [codigoconjuan](https://codigoconjuan.com), donde aprendí las bases de `useReducer` y `Context API`.

## Conclusión

La migración a **Context API** ha sido una excelente lección en la optimización y simplificación de aplicaciones React. Este proyecto me permitió entender mejor la importancia de manejar el estado de manera global y cómo eso puede mejorar tanto el rendimiento como la mantenibilidad del código.
