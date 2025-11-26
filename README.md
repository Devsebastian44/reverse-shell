## Reverse Shell

<p align="center">
  <img src="./Img/Logo.png" height="300px" width="350px">
</p>

Una **reverse shell** es una técnica utilizada en ciberseguridad que permite establecer una conexión entre un atacante y una máquina objetivo, otorgando acceso remoto para ejecutar comandos. Este proyecto incluye scripts para configurar una reverse shell en **Windows** y **Linux** con fines educativos.

---

## ⚙️ Requisitos

- Linux (Ubuntu/Kali recomendado)
- Python 3.8 o superior
- Visual Studio Code (para edición en Windows)
- Netcat (para escuchar conexiones en Linux)

---

## 🚀 Instalación

Clona el repositorio y accede al directorio:

```bash
git clone https://github.com/Devsebastian44/Reverse-Shell.git
cd Reverse-Shell
```

---

## ▶️ Uso

En la máquina del atacante linux se debe ejecutar el siguiente comando:


### Linux

Ejecuta el archivo de configuración:

```bash
sudo chmod +x config.sh
sudo bash config.sh
```


Configura la IP del atacante en `shell.py` (Windows) o `shell.sh` (Linux) dependiendo a que máquina se va atacar:

<p align="center">
  <img src="./Img/config2.png">
</p>

Luego escucha la conexión con netcat en Linux (máquina atacante):

```bash
nc -lvnp 4444
```

---

## 📂 Estructura del proyecto

```
Reverse-Shell/
│── scripts/           # Carpeta con los scripts de la reverse shell
│   │── shell.py       # Script de reverse shell para Windows
│   │── shell.sh       # Script de reverse shell para Linux
│── config.sh          # Configuración inicial
``` 

---

## 📜 Licencia

Este proyecto está bajo la licencia MIT. Puedes usarlo libremente con fines educativos y de investigación.

---

## ⚠️ Aviso

Este script ha sido desarrollado únicamente con fines **educativos y de investigación en ciberseguridad**. El uso indebido de este material puede ser **ilegal**. No me responsabilizo del mal uso ni de los daños que puedan ocasionarse por su ejecución.
