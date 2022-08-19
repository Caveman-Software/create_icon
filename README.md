# create_icon 0.4.3

## <img src="https://raw.githubusercontent.com/Caveman-Software/mygui/main/Icon.png" width="35" height="35">  Caveman Software® 2022

Released 8/17/22

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

The above example allows the icon to be place in the menubar

<img src="https://github.com/Caveman-Software/create_icon/blob/main/Capture.PNG?raw=true" width="95" height="95">
