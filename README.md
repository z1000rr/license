# Licencia para Sublime Text build 4143
1. Ir a https://hexed.it/
2. Hacer clic en el botón "Abrir archivo" en la parte superior izquierda y seleccionar sublime_text (ubicado en: **/opt/sublime_text/sublime_text**)
3. Regresar a hexed.it y en la parte superior derecha veremos la etiqueta del buscador, donde introduciremos el siguiente código: **80 78 05 00 0F 94 C1**
4. El código se subrayará y debemos reemplazarlo uno por uno por el siguiente: **C6 40 05 01 48 85 C9**
5. Hacer clic en el botón "Guardar como" y guardar en la carpeta de descargas.
6. Abrir la terminal y escribir los siguientes comandos:

```bash
sudo mv /opt/sublime_text/sublime_text ./sublime_text.old    # Renombrar sublime_text antiguo a sublime_text.old
cd $HOME/Downloads/    # Entrar en la carpeta Descargas
sudo chmod 755 sublime_text    # Dar permisos al "nuevo" sublime_text
sudo chown root sublime_text    # Cambiar el propietario del archivo a "root"
sudo chgrp root sublime_text    # Cambiar el grupo propietario a "root"
sudo mv sublime_text /opt/sublime_text/    # Mover el nuevo sublime_text al directorio original
```
Si volvemos a abrir el Sublime Text ya deberíamos tener la licencia.
Para confirmarlo debemos ir a la parte superior **"Help > About Sublime Text"** y debería aparecer el mensaje "Unlimited Uer Lcence".

### ¡Listo! Espero que les sirva de ayuda
