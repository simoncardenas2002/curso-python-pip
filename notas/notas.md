# Entornos virtuales (ENV)
Estos entornos nos permiten trabajar con unas versiones
específicas en cada diferente proyecto, esto porque es necesario
a la hora de trabajar en entornos colaborativos poder tener 
ambientes no siempre compartidos 

Verificar donde esta python y pip
"""sh
which python3

which pip3
"""
Si estas en linus o wsl debes instalar
""" sh
sudo apt install -y python3-venv
"""
Poner cada proyecto en su propio ambiente, entrar en cada carpeta.
"""sh
python3 -m venv env
"""
Activar el ambiente
"""sh
source env/bin/activate
"""
Salir del ambiente virtual

deactivate
Podemos instalar las librerias necesarias en el ambiente virtual como por ejemplo
"""sh
pip3 install matplotlib==3.5.0
"""
Verificar las instalaciones
"""sh
pip3 freeze
"""



# Archivo Requirements.txt 
este archivo nos permite que a la hora de trbajar
colaborativamente , podamos instalar en nuestro entorno
unas dependencias específicas para evitar tener conflictos
por las diferentes versiones de las librerias instaladas.

Generar el archivo con el siguiente comando

"""sh
pip3 freeze > requirements.txt
"""
Revisar lo que hay dentro del archivo

"""sh
cat requirements.txt
"""
Instalar las dependencias necesarias para contribuir más rápido en proyectos

"""sh
pip3 install -r requirements.txt
"""
Preparar archivo para contribución

