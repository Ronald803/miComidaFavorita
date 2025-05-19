## Instrucciones de instalación

- Una vez que se tenga el repositorio en local, ejecutar en consola el siguiente comando

```
npm i
```

- Para correr el proyecto ejecutar en consola el siguiente comando

```
npx expo start
```

## Descripción de mejoras implementadas

- Se creó folder utils, donde se almacenará el file "validations.js"
- Dentro de validations.js están las funciones:
  - validatePassword
  - validateEmail

#### RegisterScreen.js

- Se añadieron los estados:
  - isErrorEmail
  - isErrorPassword
  - isErrorConfirmPassword
  - isLoading
- Mediante useEffects se ejecutan los validadores de los diferentes campos
- Se añadió el Input para la confirmación de la contraseña
- Gracias a los estados y validación se agregaron mensajes de error en caso de que un estado de error sea verdadero
- Gracias a la prop disabled del Button Registrarse se deshabilita este botón mediante un OR entre los diferente estados de errores
- Gracias al estado isLoading, mediante un condicional se despliega un indicador de carga o el Botón de Registrarse, ya sea cuando se esté ejecutandose o no

#### LoginScreen.js

- Se añadieron los siguientes estados
  - isErrorEmail
  - isLoading
- Mediante useEffect se ejecuta la validación de correo electrónico
- Gracias al estado y validación de email y contraseña se agregaron mensajes de error en caso de que un estado de error sea verdadero y se deshabilitan los botones
- Gracias al estado isLoading, mediante un condicional se despliega un indicador de carga o el Botón de Iniciar sesión, ya sea cuando se esté iniciando sesión o no

#### HomeScreen.js

- Se añadieron los siguientes estados
  - isProfileLoading
  - isUpdateLoading
- Gracias a los estados loading (isProfileLoading, isUpdateLoading), mediante un condicional se despliega un indicador de carga o los Inputs, y el botón Actualizar Perfil, ademas de que se deshabilitan los botones con la prop disabled

## Screenshots de la aplicación
