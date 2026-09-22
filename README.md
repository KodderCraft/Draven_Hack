# 🏴‍☠️ Draven_Hack

> Bot de WhatsApp basado en **Baileys** con sistema modular, aliases dinámicos, actualización remota y herramientas de administración para el Owner y SuperOwner.

---

# 🚀 Características

### 👁️ Recuperación de View Once

Permite recuperar contenido de "Ver una sola vez":

* 📸 Imágenes
* 🎥 Videos
* 🎵 Audios

---

### 🏷️ Sistema de Aliases

Añade nuevos aliases directamente desde WhatsApp.

Ejemplo:

```bash
addalias menu help
addalias vv ver
```

Los aliases se cargan automáticamente y aparecen en el menú.

---

### 👑 Sistema Owner + SuperOwner

El bot soporta dos niveles de acceso:

#### Owner

* Se obtiene automáticamente desde la sesión.
* Es el propietario de la instancia instalada.

#### SuperOwner

* Configurado desde `config.js`.
* Tiene acceso a todas las instancias del bot.
* Compatible con números normales y LID de WhatsApp.

---

### 🔄 Actualizaciones Remotas

Los usuarios pueden actualizar el bot desde WhatsApp.

```bash
update
```

El sistema ejecuta:

```bash
git pull
npm install
```

y reinicia automáticamente el bot.

---

### ♻️ Reinicio Remoto

```bash
restart
```

Reinicia el bot automáticamente.

Compatible con PM2.

---

### 📂 Sistema Modular

Los comandos se cargan automáticamente desde las carpetas:

```text
commands/
```

No es necesario editar el núcleo del bot para añadir nuevas funciones.

---

# 📂 Estructura del Proyecto

```text
Draven_Hack/
├── auth_info/
├── commands/
│   ├── Añadidor_de_Aliases/
│   │   └── addalias.js
│   ├── media/
│   │   └── vv.js
│   ├── menu/
│   │   └── menu.js
│   ├── Owner/
│   │   ├── restart.js
│   │   └── update.js
│   └── private/
│       └── push.js
├── plugins/
│   └── antiDelete.js
├── config.js
├── index.js
├── logger.js
└── package.json
```

---

# 📥 Instalación

## 📱 Android (Termux)

```bash
pkg update && pkg upgrade -y
```
```bash
pkg install git nodejs -y
```
```bash
termux-setup-storage
```
```bash
git clone https://github.com/KodderCraft/Draven_Hack
```
```bash
cd Draven_Hack
```
```bash
npm install
```
```bash
node index.js
```

---

## 💻 Windows / Linux

```bash
git clone https://github.com/KodderCraft/Draven_Hack
```
```bash
cd Draven_Hack
```
```bash
npm install
```
```bash
node index.js
```

---

# ⚙️ PM2 (Recomendado)

Instalar PM2:

```bash
npm install -g pm2
```

Iniciar el bot:

```bash
pm2 start index.js --name draven
```

Ver logs:

```bash
pm2 logs draven
```

Guardar configuración:

```bash
pm2 save
```

---

# 📋 Comandos Disponibles

### Menú

```bash
menu
```

---

### Recuperar View Once

```bash
vv
```

---

### Añadir Alias

```bash
addalias [comando] [alias]
```

Ejemplo:

```bash
addalias menu help
```

---

### Actualizar Bot

```bash
update
```

---

### Reiniciar Bot

```bash
restart
```

---

# 🔐 Seguridad

⚠️ Nunca compartas:

```text
auth_info/
session.json
```

Estos archivos contienen las credenciales de tu sesión de WhatsApp.

---

# ⚠️ Descargo de Responsabilidad

Este proyecto ha sido desarrollado con fines educativos, de investigación y uso personal.

El autor no promueve, aprueba ni se hace responsable del uso indebido de esta herramienta, incluyendo pero no limitado a:

* Violación de la privacidad de terceros.
* Acceso no autorizado a información ajena.
* Incumplimiento de los términos de servicio de WhatsApp.
* Actividades ilegales o contrarias a la legislación vigente.

El uso de este software es responsabilidad exclusiva del usuario final.

Al utilizar Draven_Hack, aceptas que cualquier consecuencia derivada de su uso recaerá únicamente sobre quien lo ejecute o distribuya.

---

# 🔐 Advertencia de Seguridad

Nunca compartas ni publiques los siguientes archivos:

```text
auth_info/
session.json
```

Estos contienen credenciales y claves necesarias para acceder a tu sesión de WhatsApp.

La exposición de estos archivos puede permitir que terceros obtengan acceso completo a tu cuenta.


# 👨‍💻 Autor

**BrayanRK**

GitHub:
https://github.com/BrayanRK
