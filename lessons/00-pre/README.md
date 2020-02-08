# Requerimientos para seguir el curso

Para poder realizar el curso debes instalar una serie de aplicaciones en tu Laptop las cuales se detallan a continuacion.

# Crear llave SSH

Debes crear tu llave SSH para poder clonar y realizar operations con Git. Las instrucciones estan documentadas en el siguiente enlace `https://wiki.archlinux.org/index.php/SSH_keys`. Te recomendamos crear una llave privada `ed25519` o llave RSA de al menos `3076` bits.

Una vez creada la llave debes agregarla a tu agente SSH con el siguiente comando:

```
$ ssh-add .ssh/id_ed25519.pub
```

> :warning: Recuerda proteger y **nunca** compartir tu llave privada!

# Crear cuenta en GitHub

Para acceder al contenido del curso debes tener una cuenta en github.com. El primer paso es ir al siguiente enlace `https://github.com/join` y completar todos los campos.

Una vez completado debes agregar tu llave publica SSH previamente creada. Las instrucciones estan disponibles en `https://help.github.com/en/enterprise/2.16/user/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account`.

# Crear cuenta en Amazon Web Services

Amazon permite crear una cuenta gratuita y acceder a algunos servicios de forma gratuita. Para poder
realizar los ejercicios es **mandatorio** crear una cuenta. Ten en consideracion que a pesar que la cuenta es gratis AWS te pedira tu tarjeta de credito (visa). Si no sabes lo que haces, puedes recurrir en costos extras asociados al uso asi que por favor ten cuidado. 

El link para poder crear la cuenta es `https://aws.amazon.com/free/start-your-free-trial/`. Una vez creada tu cuenta por favor lee las mejores practicas para asegurar tu cuenta `https://aws.amazon.com/blogs/security/getting-started-follow-security-best-practices-as-you-configure-your-aws-resources/`.

En resumen lo que debes hacer es (para efectos del curso) es:

- Activar Two Factor Authentication (usa [Authy](https://authy.com/) o si puedes un token fisico)
- Crear un password que sea muy fuerte (con tu aplicacion)
- Crear `access keys` para tu usuario (asi podremos usar la API/AWS CLI)

# TerraForm

Terraform es una herramienta que nos permite administrar el codigo de infrastructure (Infrastructure as Code) de manera mas eficiente y humana. Terraform interactua con las API de AWS de manera y el lenguaje utilizado es HCL (HashiCorp Configuration Language). Las instrucciones para instalar Terraform han sido documentadas en [este](https://learn.hashicorp.com/terraform/getting-started/install.html) enlace.

# Visual Studio Code

Visual Studio Code es sin duda el editor de texto con interfaz grafica mas popular en este momento, gratuito y multi plataforma. Las instrucciones para instalar la aplicacion estan disponibles en la [documentacion](https://code.visualstudio.com/docs/setup/linux) oficial.

Algunos plugins que te recomendamos instalar:

- GitLens
- Terraform

# Docker

Durante el curso empaquetaremos nuestro software en containers, por lo cual debes instalar Docker en tu laptop. Las instrucciones estan bien documentadas en `https://docs.docker.com/install/`. Para el caso de Kubernetes usaremos `minikube` que nos hara la vida mas facil para probar algunos workloads, las instrucciones estan en `https://kubernetes.io/docs/setup/learning-environment/minikube/`.