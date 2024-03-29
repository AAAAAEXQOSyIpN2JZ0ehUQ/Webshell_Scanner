![logo](https://edteam-media.s3.amazonaws.com/blogs/big/2ab53939-9b50-47dd-b56e-38d4ba3cc0f0.png)

# Webshell Scanner

## :information_source: Descripci�n
Este script en Python es un esc�ner de webshells que se encarga de identificar 
la presencia de webshells en un sitio web dado. Utiliza una lista de nombres 
de archivos comunes asociados con webshells y realiza solicitudes HTTP para 
verificar su existencia en el sitio web objetivo. Una vez encontradas, 
muestra las URL de las webshells encontradas.

## :arrow_down: Instalacion

1. Clona este repositorio en tu m�quina:

    ```python
    git clone https://github.com/JennValentine/Webshell_Scanner.git
    ```
2. Navega al directorio del repositorio:
    ```python
    cd Webshell_Scanner
    ```

## :hammer: Modo de Uso

Ejecutar el script con la siguiente sintaxis:

```python3
python3 webshell_scanner.py -u URL -s WORDLIST_FILE [-o OUTPUT_FILE]
```

* -u o --url: Especifica la URL del sitio web objetivo.
* -s o --shell: Especifica la ruta al archivo que contiene una lista de nombres de archivos de webshells.
* -o o --output (opcional): Permite guardar la salida en un archivo.

Ejemplo de uso b�sico:

```python
python3 webshell_scanner.py -u http://example.com -s shelllist.txt
```

Ejemplo con guardado de salida:

```python
python3 webshell_scanner.py -u http://example.com -s shelllist.txt -o found_shells.txt
```

## :busstop: Ayuda 

Ejecutar el script con argumentos -h o --help:

```bash
python3 webshell_scanner.py -h
```

:bookmark_tabs: Este script realiza solicitudes HTTP para verificar la existencia de webshells en un sitio web. 
�salo con precauci�n y aseg�rate de tener permiso para escanear el sitio web objetivo.

## :octocat: Cr�ditos
1. [Jenn Valentine](https://t.me/JennValentine) - Update Contributor
