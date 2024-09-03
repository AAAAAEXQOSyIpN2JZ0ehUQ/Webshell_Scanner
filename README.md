![logo](https://img.freepik.com/vector-premium/pelirroja-anime-error-404-pagina-no-encontrada_150972-657.jpg?w=826)

# Webshell Scanner

## :information_source: Descripci�n
Este script en Python es un esc�ner de webshells que se encarga de identificar 
la presencia de webshells en un sitio web dado. Utiliza una lista de nombres 
de archivos comunes asociados con webshells y realiza solicitudes HTTP para 
verificar su existencia en el sitio web objetivo. Una vez encontradas, 
muestra las URL de las webshells encontradas, ademas cuenta con una herramienta 
complementaria un script para realizar un escaneo de directorios utilizando Dirb.

## :computer: Instalaci�n

1. Clona este repositorio en tu m�quina:
    ```python
    git clone https://github.com/JennValentine/Webshell_Scanner.git
    ```
2. Navega al directorio del repositorio:
    ```python
    cd Webshell_Scanner
    ```
3. Instalaci�n de requerimientos:
    ```python
    python3 -m pip install -r requirements.txt
    ```

## :computer: Instalaci�n en una L�nea
```bash
wget https://raw.githubusercontent.com/JennValentine/Webshell_Scanner/main/install.sh; sudo chmod +x install.sh; sudo ./install.sh; sudo rm -rf install.sh
```

## :sos: Ayuda 

Ejecutar el script con argumentos -h, --help para desplegar la ayauda de argumentos:

```python
python3 webshell_scanner.py -h
```
```
webshell_scanner.py [-h] -u URL -s SHELL [-d DIRECTORIES] [-o output_file]

Argumentos:

* -u URL, --url URL: Especifica la URL del sitio web objetivo.
* -s SHELL_FILE, --shell SHELL_FILE: Especifica la ruta del archivo que contiene la lista de nombres de shell.
* -d DIRECTORIES_FILE, --directories DIRECTORIES_FILE: (Opcional) Especifica la ruta del archivo que contiene los directorios a escanear en busca de shells.
* -o OUTPUT_FILE, --output OUTPUT_FILE: (Opcional) Guarda la salida en un archivo.
```

## :rocket: Modo de Uso para webshell scanner

Para utilizar el webshell scanner, ejecuta el script webshell_scanner.py desde la l�nea de comandos con los par�metros adecuados, como la URL del sitio web objetivo y la ruta del archivo de lista de nombres de archivos de webshells.

Ejemplo de uso:

```python
python3 webshell_scanner.py -u http://example.com/ -s shelllist.txt
```

Ejemplo de uso con guardado de salida:

```python
python3 webshell_scanner.py -u http://example.com/ -s shelllist.txt -o found_shells.txt
```

Ejemplo de uso con directorios guardados por 'dirb script':
```python
python3 webshell_scanner.py -u http://example.com/ -s shelllist.txt -d directorios_encontrados.txt
```

Ejemplo de uso con directorios guardados por 'dirb script' con guardado de salida:

```python
python3 webshell_scanner.py -u http://example.com/ -s shelllist.txt -d directorios_encontrados.txt -o found_shells.txt
```
![logo](https://github.com/JennValentine/Webshell_Scanner/blob/main/Imagenes/webshell_scanner.jpg)

:memo: Notas: El webshell scanner se encarga de identificar la presencia de webshells en un sitio web dado. Utiliza una lista de nombres de archivos comunes asociados con webshells y realiza solicitudes HTTP para verificar su existencia en el sitio web objetivo. Una vez encontradas, muestra las URL de las webshells encontradas.

## :rocket: Modo de Uso para dirb script

Para utilizar el dirb script, ejecuta el script dirb script desde la l�nea de comandos con la URL del sitio web que deseas escanear como �nico argumento.

Ejemplo de uso:

```python
python3 dirb_script.py http://example.com/
```
![logo](https://github.com/JennValentine/Webshell_Scanner/blob/main/Imagenes/dirb_script.jpg)

:memo: Notas: El dirb script se utiliza para realizar un escaneo de directorios en una URL especificada. Utiliza la herramienta Dirb para realizar el escaneo y captura los directorios y archivos encontrados durante el proceso. Los resultados se guardan en archivos de texto para su posterior an�lisis.

## :email: Contacto
* :busts_in_silhouette: [Jenn Valentine](https://t.me/JennValentine) - Update Contributor :octocat: