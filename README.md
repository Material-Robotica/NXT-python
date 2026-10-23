# Programar el NXT en Python con nxt-python 🐍🤖

Guía para controlar los robots **LEGO MINDSTORMS NXT** desde la computadora con **Python**, usando la librería [nxt-python](https://ni.srht.site/nxt-python/latest/), **sin cambiar el firmware original de LEGO**. Pensada para Ubuntu.

## 🌐 Ver la guía

👉 **[Abrir la guía](https://material-robotica.github.io/NXT-python/GuiaNXT-python.html)**

> ⚠️ **Estado:** guía armada a partir de la documentación oficial de nxt-python 3. Todavía no se probó en la sala.

## ¿Cómo funciona?

El programa en Python corre en la computadora y le envía órdenes al NXT por USB (o Bluetooth), una por una. Es distinto de leJOS, donde el programa se copia al NXT y corre dentro de él.

| | leJOS (Java) | nxt-python |
|---|---|---|
| Dónde corre el programa | En el NXT | En la computadora |
| Firmware del NXT | leJOS (hay que instalarlo) | El original de LEGO (no se toca) |
| Sirve también para Open Roberta | No, hasta reinstalar el de LEGO | Sí |
| Robot sin cable | Sí, una vez subido el programa | Solo con Bluetooth |
| Pantalla del NXT | Muestra mensajes | Los mensajes salen en la computadora |

## 📚 Contenido

**Instalación (Ubuntu)**
1. Comprobar el firmware del NXT
2. Instalar Python y nxt-python (en un entorno virtual)
3. Dar permiso de acceso al NXT por USB (regla udev)
4. Probar la conexión con `nxt-test`

**Programar**

5. Primer programa
6. Motores
7. Sensores (contacto, luz y ultrasónico)
8. Explorador que esquiva obstáculos
9. Una clase `Robot` en Python, para comparar con POO en Java

Incluye además una sección de problemas frecuentes y una nota sobre Windows.

## ⚡ Inicio rápido

```bash
sudo apt update
sudo apt install python3-venv python3-pip libusb-1.0-0
python3 -m venv ~/nxt-env
source ~/nxt-env/bin/activate
pip install --upgrade nxt-python
nxt-test
```

Los pasos completos, incluido el permiso USB, están en la guía.

## 🔗 Material relacionado

- [NXT-java](https://github.com/Material-Robotica/NXT-java): programar el NXT en Java con leJOS.
- [Documentación oficial de nxt-python](https://ni.srht.site/nxt-python/latest/)

## 👩‍🏫 Autora

Prof. Elizabeth Izquierdo · [Material-Robotica](https://github.com/Material-Robotica)
