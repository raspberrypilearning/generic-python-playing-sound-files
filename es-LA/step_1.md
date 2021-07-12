
Para reproducir un archivo de sonido con Python, puedes usar un módulo llamado `pygame`. Viene preinstalado en la Raspberry Pi, pero si estás en otro sistema operativo, es posible que debas usar [pip](https://pip.pypa.io/es-LA/stable/installing/) para instalarlo. En Linux y MacOS, puedes abrir una terminal y escribir:

```bash
sudo pip3 install pygame
```

En Windows puedes abrir PowerShell y escribir:

```bash
pip3 install pygame
```

### Importar e inicializar pygame

- Primero deberás importar el módulo `pygame` e inicializarlo.

 ```python
 import pygame
 pygame.init()
 ```

### Reproducir un sonido

- A continuación puedes crear un objeto de `sonido`, dándole la ruta de tu archivo.

 ```python
 mi_sonido = pygame.mixer.Sound('ruta/a/mi/archivo de sonido.wav')
 ```

- Luego puedes reproducir el sonido.

 ```python
 mi_sonido.play()
 ```
