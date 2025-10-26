## ¿Cuál es la diferencia entre autenticación y autorización?

**Autenticación** es verificar **quién eres**. Es el proceso de validar la identidad del usuario, típicamente mediante credenciales como usuario y contraseña.

**Autorización** es verificar **qué puedes hacer**. Es el proceso de determinar qué permisos o accesos tiene un usuario ya autenticado dentro del sistema.
## ¿Cuál es la función del token JWT en la guía?

El **JWT (JSON Web Token)** sirve como mecanismo de autenticación que permite identificar al usuario en cada petición sin mantener sesiones en el servidor.

**Funcionamiento:**
1. El usuario inicia sesión con sus credenciales
2. El servidor genera un JWT firmado con información del usuario
3. El cliente guarda el token y lo envía en cada petición posterior
4. El servidor verifica el token y permite o deniega el acceso