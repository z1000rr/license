# Licencia para Sublime Text build 4143

Para obtener una licencia ilimitada de Sublime Text en Linux, debemos seguir los siguientes pasos:

1. Ir a https://hexed.it/
2. Hacer clic en el botón "Abrir archivo" en la parte superior izquierda y seleccionar sublime_text (ubicado en: /opt/sublime_text/sublime_text)
3. Regresar a hexed.it y en la parte superior derecha veremos la etiqueta del buscador, donde introduciremos el siguiente código: 80 78 05 00 0F 94 C1
4. El código se subrayará y debemos reemplazarlo uno por uno por el siguiente: C6 40 05 01 48 85 C9
5. Hacer clic en el botón "Guardar como" y guardar en la carpeta de descargas.
6. Abrir la terminal y escribir los siguientes comandos:
    ```sh
sudo mv /opt/sublime_text/sublime_text ./sublime_text.old    # Renombrar sublime_text antiguo a sublime_text.old
cd $HOME/Downloads/    # Entrar en la carpeta Descargas
sudo chmod 755 sublime_text    # Dar permisos al "nuevo" sublime_text
sudo chown root sublime_text    # Cambiar el propietario del archivo a "root"
sudo chgrp root sublime_text    # Cambiar el grupo propietario a "root"
sudo mv sublime_text /opt/sublime_text/    # Mover el nuevo sublime_text al directorio original

    ```







---> for unlimited user license in linux
file bash "sublime_text" is in /opt/sublime_text/sublime_text
first go to site https://hexed.it/
click on Open file and put file "sublime_text"
go to section Search in left of page
put 80 78 05 00 0F 94 C1 in label Search for
then click on Find next
after find it then change if one by one to C6 40 05 01 48 85 C9
after that click on Export
then write this command in terminal
sudo mv /opt/sublime_text/sublime_text ./sublime_text.old cd $HOME/Downloads/ chmod 755 sublime_text sudo chown root sublime_text sudo chgrp root sublime_text sudo mv sublime_text /opt/sublime_text/

Done Happy Code (^-^)
