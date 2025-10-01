🇦🇷 Mapa de Dirección del Drone (opcional con punto manual de referencia)<br>
Version 0.3 - Versión MS Windows

¿Qué hace?<br>
📍 Extrae la ubicación y orientación del drone desde una imagen aérea (JPG, PNG o DNG) usando ExifTool<br>
📏 Dibuja una línea de dirección desde el drone hacia donde apunta, con longitud configurable<br>
🎯 Opcionalmente compara con un objetivo manual (como Colonia del Sacramento) y calcula distancia y ángulo<br>
🗺️ Genera un mapa interactivo HTML con capas globales (calles, claro, oscuro, satélite alternativa)<br>
🌀 Archivo de salida de nombre configurable

> Esta versión procesa un archivo por vez.

> Testeado con DJI Air 3S, debería ser compatible con todos los DJI y otras marcas que utilicen el perfil estarandizado XPM en las imágenes.

🖥️ ¿Qué necesito?
- El archivo con el código (gdrone_direction_mapperXX.py)
- Python (https://www.python.org/downloads) + Folium para Phyton (línea de comandos en Windows, ejecutar: "pip install folium")
- Descargar ExifTool (https://exiftool.org/), el que dice Windows 32 o 64-bit.
- Descomprimir "exiftool(-k).exe" y el directorio "/exiftool_files"/ en el mismo directorio que colocaremos "gdrone_direction_mapperXX.py" y las imágenes a evaluar.
- Renombrar "exiftool(-K).exe" a "exiftool.exe"

 > El XX en "gdrone_direction_mapperXX.py" corresponde a la última versión disponible.  Las versiones anteriores se van eliminando.

⚠️ ¿Qué elementos son de configuración OBLIGATORIA?
- jpg_path: ruta del archivo de imagen con metadatos GPS
- distance_value: número, longitud de la línea en metros o kilómetros
- distance_unit: "m" o "km" según la unidad elegida, metros o kilómetros

🧩 Parámetros opcionales / Optional user options
- manual_lat y manual_lon: coordenadas del objetivo manual (usar None si no se desea)
- gimbal_rotates_yaw: si el gimbal controla el giro horizontal (True o False)
- gimbal_rotates_pitch: si el gimbal controla el ángulo vertical (True o False)
- use_custom_filename: si se desea que el archivo HTML se nombre automáticamente según la imagen (True o False)

👨‍💻 Código
- Descargá gdrone_direction_mapperXX.py
- Recordá editar "gdrone_direction_mapperXX.py" para ajustarlo a tus preferencias e indicar el nombre de la fotografía a evaluar.
- Colocá las imágenes en el mismo directorio que "gdrone_direction_mapperXX.py" y el ExifTool.exe y el directorio "/exiftool_files"/ 
- Ejectuar "python gdrone_direction_mapperXX.py" desde la línea de comandos o doble click desde el Explorador de Windows
- El código responderá con el resultado.

----

🇺🇸 Drone Heading Mapper (with optional reference point)<br>
Version 0.3 - MS Windows version

What does it do?<br>
📍 Extracts drone location and heading from aerial image metadata<br>
📏 Draws a heading line from the drone with customizable length<br>
🎯 Optionally compares with a manual target and calculates distance and angle<br>
🗺️ Generates an interactive HTML map with global layers<br>
🌀 Custom file name output

> This version processes one file at a time.

> Tested with a DJI Air 3S, it should be compatible with all DJI models and other brands that use standarized XPM profiles in their images.

🖥️ What do I need?
- File with the code (gdrone_direction_mapperXX.py)
- Python (https://www.python.org/downloads)
- Folium in Python (Run Windows command line: "pip install folium")
- ExifTool: https://exiftool.org — Windows 32 or 64-bit.
- Decompress "exiftool(-K).exe" and "/exiftool_files"/ to the same folder where you saved "gdrone_direction_mapperXX.py" and pictures will be placed for evaluation.
- Rename "exiftool(-K).exe" to "exiftool.exe"

> The XX in "gdrone_direction_mapperXX.py" corresponds to the latest available version for downloading.  Older versions are deleted.

⚠️ What are the MANDATORY configuration parameters?
- jpg_path: Path to the image file with GPS metadata
- distance_value: Number, line length in meters or kilometers
- distance_unit: "m" or "km", line length in meters or kilometers

🧩 Parámetros opcionales / Optional user options
- manual_lat y manual_lon: Manual target coordinates (use None to disable)
- gimbal_rotates_yaw: Whether the gimbal controls horizontal yaw (True o False)
- gimbal_rotates_pitch: Whether the gimbal controls vertical pitch (True o False)
- use_custom_filename: Whether to auto-name the HTML file based on the image (True o False)

👨‍💻 Code
- Download gdrone_direction_mapper.py
- Edit "gdrone_direction_mapperXX.py" to adjust preferences and specify the name of the photo to analyze
- Place the image(s) in the same folder as "gdrone_direction_mapperXX.py", ExifTool.exe and "/exiftool_files"/ directory
- Run "python "gdrone_direction_mapperXX.py" from the command line or double-click it from Windows File Explorer
- The code will respond with the result
