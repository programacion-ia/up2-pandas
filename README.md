# UP2 · Pandas

Programación de IA · CE IABD

Ejemplos de la unidad 2: un notebook por presentación, con los mismos ejemplos y en el mismo orden, y los datos que se usan en toda la unidad.

## Qué hay en el repositorio

```
up2-pandas/
├── datos/
│   ├── pisos.csv          600 anuncios de alquiler en Benidorm
│   ├── pisos_sucio.csv    los mismos anuncios tal como llegan, con errores
│   └── barrios.csv        zona y distancia a la playa de cada barrio
├── UP2.1 - Ejemplos.ipynb
├── UP2.2 - Ejemplos.ipynb
├── UP2.3 - Ejemplos.ipynb
└── pyproject.toml         dependencias del proyecto
```

Los datos son **simulados**: los barrios son reales, pero los anuncios y los precios se han generado con NumPy.

## Puesta en marcha (solo la primera vez)

Necesitas Git, [uv](https://docs.astral.sh/uv/) y Visual Studio Code. En Windows, trabaja dentro de WSL.

1. Clona el repositorio y entra en la carpeta:

   ```bash
   git clone https://github.com/programacion-ia/up2-pandas.git
   cd up2-pandas
   ```

2. Crea el entorno e instala las dependencias. uv descarga también la versión de Python que necesita el proyecto:

   ```bash
   uv sync
   ```

3. Abre la carpeta en VS Code e instala las extensiones que te recomienda (Python, Pylance y Jupyter):

   ```bash
   code .
   ```

4. Abre un notebook y, arriba a la derecha, elige como kernel el entorno `.venv` de la carpeta.

5. Ejecuta las celdas de una en una, de arriba abajo: cada una usa variables de las anteriores.

## Cómo trabajar con los ejemplos

- **No edites los notebooks de ejemplo.** Para probar cosas, copia el notebook a una carpeta `mis_pruebas/` y trabaja en la copia. Esa carpeta no se sube a GitHub y nunca choca con los cambios del profesor.
- **Las rutas parten de la raíz del proyecto** (`Path("datos") / "pisos.csv"`), también desde `mis_pruebas/`: VS Code está configurado para ello.
- **Las últimas celdas de cada notebook dan error a propósito.** Sirven para ver los errores más habituales.

## Cuando haya un tema nuevo

```bash
git pull
uv sync
```

`git pull` descarga los notebooks nuevos y `uv sync` instala lo que haga falta si han cambiado las dependencias.

## Si no consigues instalarlo en tu ordenador

Puedes abrir el repositorio en GitHub Codespaces, que es VS Code en el navegador con todo ya instalado: en la página del repositorio, **Code → Codespaces → Create codespace on main**. La primera vez tarda unos minutos en preparar el entorno.
