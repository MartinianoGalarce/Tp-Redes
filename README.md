# Programación sobre Redes — TP Interactivo

Trabajo práctico teórico de la materia **Programación sobre Redes**, presentado como una página interactiva en vez de un Canva o PowerPoint tradicional.

Es un único archivo HTML (`tp-redes-interactivo.html`), sin dependencias ni instalación: se abre directo en el navegador.

##  Verlo online (recomendado)

Si este repo tiene GitHub Pages activado, entrás directo desde:

```
https://martinianogalarce.github.io/Tp-Redes/tp_gp.html
```

**¿Cómo se activa GitHub Pages?** (lo hace cualquiera de los del grupo, una sola vez)
1. En el repo de GitHub: **Settings → Pages**
2. En "Build and deployment" → Source: **Deploy from a branch**
3. Branch: `main` (o la que uses) / carpeta `/root`
4. Guardar. A los 1-2 minutos queda publicado en la URL de arriba.

##  Verlo local

No necesita servidor ni puerto, es un HTML plano:

1. Cloná o descargá el repo
2. Doble click sobre `tp-redes-interactivo.html` — se abre en tu navegador por defecto

Si preferís usar VS Code, con la extensión **Live Server** también funciona: click derecho sobre el archivo → "Open with Live Server".

> Nota: las tipografías (Space Grotesk, JetBrains Mono) se cargan desde Google Fonts, así que hace falta conexión a internet la primera vez para que se vea con el estilo completo. Sin conexión, cae a una fuente del sistema pero todo sigue funcionando igual.

##  Qué contiene

| Sección | Qué muestra | Preguntas del TP |
|---|---|---|
| **1. Laboratorio de red** | Editor interactivo: agregás PCs, switches, routers, firewalls y servidores, los conectás con cables (arrastrando), les asignás IP, y corrés una prueba real de conectividad entre dos equipos (BFS sobre el grafo armado, con lógica de subredes y bloqueo por firewall). Incluye 4 escenarios precargados para arrancar rápido. | 1–4, 13, 17–19 |
| **2. Servicios, protocolos y estándares** | Acordeón con el resto del cuestionario teórico, organizado en dos bloques. | 5, 6, 7, 10–12, 14, 15, 20, 22–32 |
| **3. Elegí el enlace** | Tabla de ranking de 6 tipos de enlace WAN por 6 criterios, más 3 escenarios con la recomendación justificada. | 21 |
| **4. Nuestra experiencia con redes** | Tarjetas editables, una por integrante, para completar la respuesta individual. | 33 |

##  Cómo usar el laboratorio (sección 1)

1. Agregá dispositivos con los botones de arriba (`+ PC`, `+ Switch`, etc.)
2. Arrastralos para acomodarlos donde quieras
3. Conectalos: arrastrá desde el punto ámbar de un dispositivo hasta otro
4. Click sobre un cable existente lo desconecta
5. Elegí origen y destino abajo y tocá **"Probar conexión"** — el resultado depende de cómo armaste la red, no está guionado

Simplificaciones a propósito (para no complicar la herramienta): switch y router no tienen IP propia, solo reenvían/rutean. Dos IPs de subredes distintas necesitan un router en el camino para verse. Un firewall en modo "bloqueando" corta cualquier ruta que pase por él.


##  Stack

HTML + CSS + JavaScript vanilla, un solo archivo, sin build ni dependencias instalables.
