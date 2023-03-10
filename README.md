# PyWebWrap
PyWebWrap is a package that allows you to run your web app easily on the desktop.

To install `pywebwrap`, simply run the following command in your terminal:

`pip install pywebwrap`

---
Supported features:
 - Run local web core files within a desktop wrapper.
 - Customize the window's title, icon, width, height, and other parameters easily.
 - Allow the window to be resizable or fixed in size.
 - Disable right-clicking on the window.
 - Hide the top or status bar of the window.
 - Clear the browser cache on startup.
 - Disable JavaScript in the browser.
 - Disable access to remote and file URLs via keyboard shortcuts.

Currently working on:
 - Handle uploads & downloads to and from the web app.
 - Call JavaScript functions from Python.
 - Handle JavaScript events with Python code.
 - Emit JavaScript events from Python.

Please refer to the docstring for a list of available attributes.

To get started, simply import the `Wrap` class from the `pywebwrap.pywebwrap` module and create an instance with the desired attributes. 
Then, call the `run()` method to start the desktop app. Here's an example:

```
from pywebwrap.pywebwrap import Wrap

app = Wrap('path/to/index.html', width=1024, height=768, expandable=False, clear_cache=False)
app.run()
```

### Supported arguments
 - html_file: The path to the HTML file to be displayed in the desktop wrapper.
 - title (optional): The title to be displayed in the window's title bar.
 - icon (optional): The path to the icon file to be displayed in the window's title bar.
 - width (optional): The width of the desktop wrapper window in pixels.
 - height (optional): The height of the desktop wrapper window in pixels.
 - expandable (optional): A boolean value indicating whether the desktop wrapper window can be resized by the user.
 - disable_right_click (optional): A boolean value indicating whether right-clicking on the desktop wrapper window is disabled.
 - hide_top_bar (optional): A boolean value indicating whether the top bar of the desktop wrapper window is hidden.
 - hide_status_bar (optional): A boolean value indicating whether the status bar of the desktop wrapper window is hidden.
 - clear_cache (optional): A boolean value indicating whether the browser cache is cleared when the desktop wrapper window is opened.
 - disable_javascript (optional): A boolean value indicating whether JavaScript is disabled in the desktop wrapper window.
 - disable_keyboard_shortcuts (optional): A boolean value indicating whether keyboard shortcuts to access remote and file URLs are disabled in the desktop wrapper window.
