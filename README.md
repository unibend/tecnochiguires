# Portafolio Web del Equipo

## Criterios de Evaluación

Para esta evaluación, nuestros criterios fueron:

- Realizar la navegación en al menos **3 páginas web** programadas en cualquier lenguaje que el equipo considere conveniente.
- Una de esas páginas debe solicitar datos y **validarlos con JavaScript**.
- Incluir **Bootstrap** en el diseño de dichas páginas.

---

## Diseño de la Página

El sitio web consiste en **7 archivos HTML estáticos**. El usuario puede navegar fácilmente entre las páginas utilizando los menús de navegación y el flujo de registro.

### Páginas principales

- **Inicio**: Contiene enlaces al resto de las páginas principales.
- **Portafolio**: Contiene información sobre los proyectos realizados por el equipo.
- **Sobre Nosotros**: Presenta información del equipo y un enlace al repositorio en GitHub.
- **Formulario**: Permite al usuario registrarse en el sistema.
- **Iniciar Sesión**: Sección accesible desde el formulario.
- **Gracias**: Mensaje de confirmación tras completar el registro.
- **Usuario**: Vista privada con los datos del usuario registrado.

### Funcionalidad del Registro

Al hacer clic en el botón de **registro**, se ejecuta código JavaScript que:

1. Revisa si el usuario ya tiene una sesión iniciada:
   - ✅ Si la tiene, se redirige a la página **Usuario**, donde puede ver su información.
   - ❌ Si no la tiene, se redirige a la página **Formulario** para registrarse.
2. Una vez registrado:
   - El usuario es redirigido a la página **Gracias**, donde se le informa que su solicitud está siendo revisada.
   - Cuando la solicitud es aprobada manualmente, la página indica que fue aceptado.
   - También puede cerrar su sesión y crear un nuevo registro.

---

## Tecnologías Utilizadas

- **HTML5** para la estructura del sitio.
- **Bootstrap** para el diseño visual responsivo.
- **JavaScript** para validación de formularios y control del flujo de usuario.
- **Firebase** como base de datos y para la autenticación de usuarios.

El código JavaScript está incluido directamente en los archivos HTML, pero está pensado para migrarse a archivos `.js` separados si el proyecto escala.

---

## Enlace a la Página Web

Accede al sitio aquí:  
🔗 [https://tecnochiguires.vercel.app/](https://tecnochiguires.vercel.app/)


---

## Cómo Ejecutar Localmente

Para correr la página en tu máquina local:

1. Descarga el código desde GitHub, o desde [esta carpeta de google drive](https://drive.google.com/drive/folders/1GGcufaJHn35b0NJ2PSzf3i-153pFQ-VQ?usp=sharing)
1. Abre una terminal y navega a la carpeta del proyecto.
2. Ejecuta el siguiente comando:

```bash
python -m http.server
```
---
## Actualización 2025-07-03
### Nueva Funcionalidad: Recuperación de Contraseña
Se ha agregado una nueva característica de **recuperación de contraseña** para mejorar la experiencia del usuario:

#### Cambios Implementados:
- **Página de Login Actualizada**: Se agregó un enlace "¿Olvidaste tu contraseña?" debajo del enlace de registro.
- **Nueva Página de Recuperación**: Se creó `reset-password.html` con diseño completamente consistente con el resto del sitio.
- **Integración con Firebase**: Implementación de la función `sendPasswordResetEmail()` para envío automático de correos de recuperación.

#### Funcionalidad:
1. El usuario hace clic en "¿Olvidaste tu contraseña?" desde la página de login.
2. Se redirige a la página de recuperación donde ingresa su correo electrónico.
3. Firebase envía automáticamente un correo con instrucciones para restablecer la contraseña.
4. El sistema maneja errores comunes (usuario no encontrado, correo inválido, etc.).
5. Se muestran mensajes de confirmación y error apropiados.


