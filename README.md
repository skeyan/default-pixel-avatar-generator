# default-pixel-avatar-generator

Note: This fork updates the original repo to be compatible with the newest version of the Python Pillow library.

This Python script uses the Pillow (PIL Fork) library to generate pixel art style images with customizable backgrounds and text overlays.

## Features

* **Multiple Color Palettes:** Includes a variety of predefined color palettes to choose from.
* **Random Pixel Backgrounds:** Creates a background by randomly selecting colors from the chosen palette for each pixel block.
* **Rainbow Background Option:** Generates a background with color gradients based on the chosen palette.
* **Text Overlay:** Allows you to add text to the generated image with customizable font size and color (using the last color in the selected palette).
* **Text Wrapping:** Automatically wraps long text to fit within the image width.
* **Customizable Image Size and Pixel Size:** Control the dimensions of the output image and the size of the individual pixel blocks.
* **Output to `/results` Folder:** Saves the generated images in a dedicated `results` folder within the script's directory.

## Requirements

* **Python 3.x**
* **Pillow Library:** Install using pip:
    ```bash
    pip install Pillow
    ```
* **(Optional) Helvetica-Bold Font:** The script attempts to use "fonts/Helvetica-Bold.ttf" for text. If this font is not found, it will fall back to a default Pillow font. You can create a `fonts` directory in the same location as the script and place a `.ttf` font file named `Helvetica-Bold.ttf` there, or modify the `draw_text` function to use a different font path.

```
    To generate images with specific parameters, you can modify the `your_script.py` file.

    This will generate an image named `image.png` in the `results` folder. It will override any prexeisting images by the same name.
```

---
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/g.png" height="250" width="250"/>
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/i.png" height="250" width="250"/>
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/t.png" height="250" width="250"/>
</p>

# Usage

```python
pixelgenerator.main(name = 'image', palette = 'purple drank', size = (500, 500), pixel = 20, rainbow = False, msg='', fontsize=250)
```

##size

```python
size = (width, height)

```
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/600 x 200.png"/>
</p>

```python
pixelgenerator.main(msg='600 x 200', size = (600, 200), fontsize=70, rainbow = True) 
```

##rainbow
`rainbow = True` or `rainbow = False`


| rainbow = True  | rainbow = False |
| ------------- | ------------- |
| <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/rainbow true.png" height="405" width="405"/>  | <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/rainbow false.png" height="405" width="405"/> |


##palette
```python
['malachite', 'deep ocean', 'ocean' , 'weed', 'palette 5', 'palette 6', 'palette 7', 'purple drank', 'hot pink', 'peach',
'fire', 'gold', 'palette 13', 'sky', 'dollar', 'palette 16', 'palette 17', 'gray', 'palette 19', 'palette 20', 'palette 21',
'palette 22', 'palette 23', 'palette 24', 'palette 25', 'palette 26', 'palette 27', 'fire on the water']
```

###malachite
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/malachite.png"/>
</p>

###deep ocean
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/deep ocean.png"/>
</p>

###ocean
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/ocean.png"/>
</p>

###weed
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/weed.png"/>
</p>

###palette 5
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 5.png"/>
</p>

###palette 6
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 6.png"/>
</p>

###palette 7
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 7.png"/>
</p>

###purple drank
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/purple drank.png"/>
</p>

###hot pink
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/hot pink.png"/>
</p>

###peach
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/peach.png"/>
</p>

###fire
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/fire.png"/>
</p>

###gold
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/gold.png"/>
</p>

###palette 13
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 13.png"/>
</p>

###sky
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/sky.png"/>
</p>

###dollar
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/dollar.png"/>
</p>

###palette 16
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 16.png"/>
</p>

###palette 17
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 17.png"/>
</p>

###gray
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/gray.png"/>
</p>

###palette 19
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 19.png"/>
</p>

###palette 20
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 20.png"/>
</p>

###palette 21
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 21.png"/>
</p>

###palette 22
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 22.png"/>
</p>

###palette 23
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 23.png"/>
</p>

###palette 24
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 24.png"/>
</p>

###palette 25
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 25.png"/>
</p>

###palette 26
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 26.png"/>
</p>

###palette 27
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/palette 27.png"/>
</p>

###fire on the water
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/fire on the water.png"/>
</p>



##msg

```python
pixelgenerator.main(msg='git', fontsize=350, rainbow = True)
```
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/git.png"/>
</p>


#python is awesome
<p align="center">
  <img src="https://raw.githubusercontent.com/vladlenomg/default-pixel-avatar-generator/master/screenshots/python is awesome.png"/>
</p>
