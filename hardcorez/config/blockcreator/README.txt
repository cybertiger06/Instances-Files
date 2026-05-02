BlockCreator - Guía rápida
==========================

1) Pon tus texturas PNG (16x16 recomendado) en:
   config/blockcreator/textures/

2) Define cada bloque con un .json en:
   config/blockcreator/blocks/

   Ejemplo (misma textura en todas las caras):
   {
     "id": "ruby_block",
     "name": "Ruby Block",
     "texture": "ruby_block.png"
   }

   Ejemplo (textura por cara):
   {
     "id": "fancy_block",
     "name": "Fancy Block",
     "faces": {
       "up":    "fancy_top.png",
       "down":  "fancy_bottom.png",
       "north": "fancy_side.png",
       "south": "fancy_side.png",
       "east":  "fancy_side.png",
       "west":  "fancy_side.png"
     }
   }

3) Reinicia el juego. Los bloques aparecerán en su propia
   pestaña del modo creativo y con /give:
     /give @s blockcreator:ruby_block

Propiedades opcionales:
  hardness (float, dureza)
  resistance (float, resistencia a explosiones)
  luminance (0-15, luz emitida)
  sound ("stone","wood","metal","glass","wool","sand","gravel")
