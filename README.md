# Easy GUI Jupyter

[![PyPI version](https://badge.fury.io/py/easy_gui_jupyter.svg)](https://badge.fury.io/py/easy_gui_jupyter)
[![Python versions](https://img.shields.io/pypi/pyversions/easy_gui_jupyter.svg)](https://pypi.org/project/easy_gui_jupyter/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Easy GUI Jupyter is a Python library that simplifies the creation of graphical user interfaces (GUIs) in Jupyter notebooks using ipywidgets. It provides a convenient way to add various types of widgets to your Jupyter notebooks, making it easier to interact with your code and visualize results.

## Features

- Simplifies the creation of GUIs in Jupyter notebooks
- Supports a variety of widget types, including labels, buttons, text inputs, sliders, checkboxes, and dropdowns
- Allows saving and loading widget values to maintain user settings across sessions
- Provides a clean and intuitive API for adding and managing widgets

## Installation

To install Easy GUI Jupyter, you can use pip:

```bash
pip install easy_gui_jupyter
```

## Usage

Here's a simple example of how to use Easy GUI Jupyter in your Jupyter notebook:

```python
from easy_gui_jupyter import EasyGUI

# Create an instance of EasyGUI
eg = EasyGUI()

# Add a text widget
eg.add_text("text", value="Hello, world!")

# Display the GUI
eg.show()
```

This will create a GUI with a single text widget displaying "Hello, world!".

You can add more widgets using the various `add_*` methods provided by the `EasyGUI` class. For example:

```python
# Add an integer slider
eg.add_int_slider("int_slider", min=0, max=10, value=5)

# Add a checkbox
eg.add_checkbox("checkbox", value=True)

# Add a dropdown
options = ["Option 1", "Option 2", "Option 3"]
eg.add_dropdown("dropdown", options=options, value=options)
```

To access the values of the widgets, you can use the `[]` operator with the widget's tag:

```python
# Get the value of the text widget
text_value = eg["text"].value

# Get the value of the integer slider
int_slider_value = eg["int_slider"].value
```

## Saving and Loading Settings

Easy GUI Jupyter allows you to save and load widget values to maintain user settings across sessions. To enable this feature, set the `remember_value` parameter to `True` when adding a widget:

```python
# Add a float slider with remembered value
eg.add_float_slider("float_slider", min=0.0, max=1.0, step=0.1, value=0.5, remember_value=True)
```

To save the current widget values, call the `save_settings()` method:

```python
# Save the current widget values
eg.save_settings()
```

The widget values will be saved to a configuration file in the user's home directory.

## Contributing

Contributions to Easy GUI Jupyter are welcome! If you find a bug, have a feature request, or want to contribute improvements, please open an issue or submit a pull request on the GitHub repository.

## License

Easy GUI Jupyter is open-source software licensed under the [MIT License](LICENSE).
