# Headless-Pi-Tkinter-GUI
A headless Raspberry Pi installation with a Tkinter GUI that loads at boot.

## Project Description

The purpose of this repo is to provide a starting point for building a simple GUI on top of a minimal OS for a Raspberry Pi.  From this starting point, you can further develop your own GIU, add additional services, etc., unique to your specific project.  
You can start with just a Raspberry Pi, SD card, and some sort of graphical display device.  My project started with a Pi 4b, a 5" TFT touchscreen, and the intent of building a stand alone temperature data logging device.  The data logger would utilize the 5" screen to provide real-time temperature data values to the user.  The services for temperature measurement and logging will be python based, so Tkinter was my choice for the GUI.  Although the Pi4 would likely have enough processing power to run my python applications and a GUI on top of the RPD desktop environment, I wanted something as efficient as possible, and would maximize the storage space available on the Pi's SD card. 
I'm sure there are probably other methods that may be smaller and more efficient, the point of this repo is not to debate that fact, but to simply provide some documentation on how to implement this particular method.  I'm not going into any further here with regard to developing the GUI beyond a simple frame with a push button, there are plenty of other resources on how to do that.  This repo will go as far as demonstrating how to get a basic Tkinter app to display on boot.

## Pros and Cons of this method:

### Pros:
1. Minimal processing and memory usage by OS, more resources available for measurements, data storage, and GUI.
2. Minimal package installation, maximum SD storage available for data storage.
3. Management of RPD, starting/running GUI on top of, and limiting user from exiting.

### Cons:
1. Developent needs to be done remotly using SSH.  I used VSCode and plug-ins for remote SSH, and python development.
2. Difficult to debug the GUI application.  I'd reccoment you develop the GUI on a seprate / full RPI environment and deploy your release version of the GUI to the envirment (production environment) described here.

## Hardware:
* Raspberry Pi 4b
* SD Card, 256Gb
* TFT Touchscreen, 5"
  
There are many touchscreens available that are compatible with a Raspberry Pi, I'm not going to go into how to install or set-up any one particular device.  The one I purchased connected to the Pi's display connector via a ribbon cable and worked without any additional configuration or drier installation.  Your device may require configuration or drives, which is beyond the scope of this repo.

## Software:
* Raspbain-Lite (Bookworm)
* X
* Python 3
* Tkinter

## Procedure
### Step 1 - Raspbian Installation
In an effort to not have to duplicate and maintain a How-To for installing Raspbian-Lite, I'll just cover the essentials here that you'll want to include.

### Step 2 - 


```bash
what to type on the command line
```

### Step 3 - 

python script...

```python
import foobar

# returns 'words'
foobar.pluralize('word')

# returns 'geese'
foobar.pluralize('goose')

# returns 'phenomenon'
foobar.singularize('phenomena')
```

### Step 4 - 

### Step 5 - 



## License

[MIT](https://choosealicense.com/licenses/mit/)
