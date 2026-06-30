# HamiTTS
Programa de codigo abierto que te ayuda a pasar de texto a audio en roblox, completamente gratis y de codigo abierto.

# Guía de Instalación y Uso
Cinco pasos rápidos para dejar HamiTTS funcionando en tu chat de voz.

Paso 1
Descargar, Extraer y Ejecutar
Descarga el archivo comprimido de HamiTTS, extrae todo su contenido en una carpeta de tu PC y ejecuta por primera vez el archivo "HamiTTS.exe".

Paso 2
Instalar Componentes Requeridos
Para que el sistema automatizado funcione, es obligatorio instalar los dos complementos necesarios: AutoHotkey y el controlador VB-Audio Virtual Cable. (despues de instalar el cable virtual, rendras que reiniciar tu computadora)

Paso 3
Configurar el Audio del Sistema
En la pestaña "Salida de Audio", presiona "Cambiar salida de audio" y sigue las instrucciones. Luego, en "Mezclador de volumen", cambia la salida de tu navegador de predeterminado a "CABLE Output" (si no vez el navegaor en mezclador de volumen, tendras que hacer que el navegador reproduzca audio para poder verlo en mezclador de volumen).

Paso 4
Iniciar HamiTTS y Elegir Voz
Selecciona tu navegador y distribución de teclado (Español/Inglés). Haz clic en "Aplicar e Iniciar", loguéate con Google en Fish Audio y elige tu voz de IA favorita en la pestaña de "Descubrimiento".

Ajustar el Micrófono en Roblox
Entra a Roblox, ve a Configuración (Settings) y en la sección de audio cambia tu Dispositivo de Entrada (Input Device) a "CABLE Output (VB-Audio Virtual Cable)".

¡Hecho!
Cada vez que presiones tu tecla de activación (/), escribas en el chat de Roblox y presiones ENTER, tu texto se transformará mágicamente en voz de IA que todos podrán escuchar.






# Seguridad y Falsos Positivos en HamiTTS (VirusTotal)
Quiero ser totalmente transparentes contigo. Si escaneas HamiTTS.exe en VirusTotal puede que aparezcan hasta 3 alertas. Aquí te explico, sin tecnicismos, por qué ocurre y por qué el programa está 100% limpio.

Cuando usas el comando pyinstaller --onefile, la herramienta agarra tu script de Python, todas las librerías (como CustomTkinter) y el propio intérprete de Python, y los mete comprimidos dentro de un ejecutable genérico llamado bootloader.
El problema es que los creadores de virus reales también usan PyInstaller para camuflar sus códigos maliciosos dentro de archivos legítimos de Python. Como consecuencia, algunos antivirus mediocres o hiper-sensibles optan por la vía fácil: marcan cualquier ejecutable creado con PyInstaller como troyano por defecto, sin importar si el código de adentro es un juego, una calculadora o mi programa.

Los antivirus modernos no solo buscan virus conocidos, sino que usan Inteligencia Artificial para analizar el comportamiento del código (detección heurística). Si analizamos lo que hace mi programa, cumple con la "lista de verificación" de lo que un troyano promedio haría:

- Entra al Registro de Windows (winreg) para husmear si AutoHotkey está instalado.

- Ejecuta procesos ocultos en el sistema (subprocess.Popen y os.startfile) para arrancar los scripts de AutoHotkey.

- Abre el navegador web de forma automática (webbrowser.open) para redirigir al usuario a Fish Audio o AutoHotkey.

- Se oculta de la pantalla (--noconsole), lo que significa que corre procesos en segundo plano sin una ventana de comandos visible.

Para un algoritmo automatizado de un antivirus, un programa que no tiene firma digital, que nadie conoce, que corre oculto, abre webs y ejecuta comandos en Windows, levanta banderas rojas inmediatamente.

Si revisas los nombres de los 3 antivirus que te dieron positivo, notarás que no son los grandes de la industria. Probablemente sean motores muy raros o poco conocidos (como MaxSecure, SecureAge, Gridinsoft, Bkav, Zillya o similares). Si los gigantes de la ciberseguridad (como Microsoft Defender, Kaspersky, Bitdefender, Avast, ESET o Symantec) dicen que el archivo está en verde (Undetected), significa que el programa está completamente limpio y seguro.



# PAGINAS OFICIALES
- Tiktok: https://www.tiktok.com/@hamirblx
- Youtube: https://www.youtube.com/@Ham44
- Pagina para descargar HamiTTS: 
