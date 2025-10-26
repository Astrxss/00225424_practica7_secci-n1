## ¿Cuál es la diferencia entre autenticación y autorización?

**Autenticación** es verificar **quién eres**. Es el proceso de validar la identidad del usuario, típicamente mediante credenciales como usuario y contraseña.

**Autorización** es verificar **qué puedes hacer**. Es el proceso de determinar qué permisos o accesos tiene un usuario ya autenticado dentro del sistema.
## ¿Cuál es la función del token JWT en la guía?

El **JWT (JSON Web Token)** permite la autenticación entre el cliente (ReactJS) y el servidor (Express) en una arquitectura headless, manteniendo la sesión del usuario sin necesidad de guardar estado en el servidor.
Funcionamiento en la guía:

**Funcionamiento:**

1. El usuario se autentica enviando credenciales al servidor Express
2. El servidor genera un JWT y lo devuelve al cliente React
3. eact guarda el token en localStorage
4. En cada petición, React envía el token mediante el middleware **verifyToken**
5. Express valida el token y permite o rechaza el acceso
