#### Playing Sound Files with Python

To play a sound file with Python, you can use a module called *Pygame*. This comes pre-installed on a Raspberry Pi, but if you are on another operating system you may need to use [pip]() to install it. On Linux and MacOS you can open a termianl and type:

~~~bash
sudo pip3 install pygame
~~~

On Windows you can open PowerShell and type:

~~~bash
pip3 install pygame
~~~

#### Importing and initialising pygame

1. To begin with you will need to import the `pygame` module and initialise it.

   ~~~python
   import pygame
   pygame.init()
   ~~~

#### Playing a sound

1. Next you can create a `Sound` object and provide it with the path to your file.

   ~~~python
   my_sound = pygame.mixer.Sound('path/to/my/soundfile.wav')
   ~~~
   
1. Lastly you can play the sound.

   ~~~python
   my_sound.play()
   ~~~
