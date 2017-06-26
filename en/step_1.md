To play a sound file with Python, you can use a module called `pygame`. It comes pre-installed on a Raspberry Pi, but if you are on another operating system you may need to use [pip](https://pip.pypa.io/en/stable/installing/) to install it.
On Linux and MacOS you can open a terminal and type:

```bash
sudo pip3 install pygame
```

On Windows you can open PowerShell and type:

```bash
pip3 install pygame
```

### Importing and initialising pygame

- First you will need to import the `pygame` module and initialise it.

   ```python
   import pygame
   pygame.init()
   ```

### Playing a sound

- Next you can create a `Sound` object and provide it with the path to your file.

   ```python
   my_sound = pygame.mixer.Sound('path/to/my/soundfile.wav')
   ```
   
- Then you can play the sound.

   ```python
   my_sound.play()
   ```
