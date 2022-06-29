# create_icon 0.4.0

## <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2022

A Simple icon to replace the tkinter feather for your programs.

----------

### Example

    import os
    from tkinter import Tk
    root=Tk()
    root.minsize(300,100)
    # Add Icon to windows Titlebar if running Windows.
    if os.name == 'nt':
        homepath = os.path.expanduser('~')
        tempFile = '%s\Caveman Software\%s' % (homepath, 'Icon\icon.ico')

        if (os.path.exists(tempFile) == True):
            root.wm_iconbitmap(default=tempFile)

        else:
            import create_icon
            print('File Created')
            root.wm_iconbitmap(default=tempFile)

    root.mainloop()

----------

The above example allows the icon to be place in the menubar as depicted below.

<img src="https://raw.githubusercontent.com/Caveman-Software/create_icon/main/Capture.PNG" width="350" height="350">

#CHANGELOG
##Version 0.4.0
Added an image to the readme file depicting the icon in a tkinter window.
##Version 0.3.9
Changed the layout of README.md to conform with Github
##Version 0.3.8
Fixed a version problem. by removing it.
##Version 0.3.7
Fixed the setup.cfg file to properly insert changelog and MIT License
##Version 0.3.6
Added changelog.md
Added License.md
Added History.md
##Version 0.3.5
Changes to CHANGELOG add
