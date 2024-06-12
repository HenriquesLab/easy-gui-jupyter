<!-- markdownlint-disable -->

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

# <kbd>module</kbd> `easy_gui_jupyter`





---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L16"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>function</kbd> `get_config`

```python
get_config(title: Optional[str]) → dict
```

Get the configuration dictionary without needing to initialize the GUI. 



**Args:**
 
 - <b>`title`</b> (str):  The title of the GUI. If None, returns the entire configuration. 



**Returns:**
 
 - <b>`dict`</b>:  The configuration dictionary. 


---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L43"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>function</kbd> `save_config`

```python
save_config(title: str, cfg: dict)
```

Save the configuration dictionary to file. 



**Args:**
 
 - <b>`title`</b> (str):  The title of the GUI. 
 - <b>`cfg`</b> (dict):  The configuration dictionary. 


---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L61"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

## <kbd>class</kbd> `EasyGUI`
A class to help simplify the creation of GUIs in Jupyter notebooks using ipywidgets. 

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L66"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `__init__`

```python
__init__(title='basic_gui', width='50%')
```

Container for widgets. 



**Args:**
 
 - <b>`title`</b> (str):  The title of the widget container, used to store settings. 
 - <b>`width`</b> (str):  The width of the widget container. 




---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L116"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_button`

```python
add_button(tag, *args, **kwargs)
```

Add a button widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L209"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_checkbox`

```python
add_checkbox(tag, *args, remember_value=False, **kwargs)
```

Add a checkbox widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L258"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_dropdown`

```python
add_dropdown(tag, *args, remember_value=False, **kwargs)
```

Add a dropdown widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 



**Example:**
 ``` gui = EasyGUI()```
    >>> gui.add_dropdown("dropdown", options=["A", "B", "C"])


---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L278"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_file_upload`

```python
add_file_upload(tag, *args, accept=None, multiple=False, **kwargs)
```

Add a file upload widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`accept`</b>:  The file types to accept. 
 - <b>`multiple`</b> (bool):  Allow multiple files to be uploaded. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L193"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_float_slider`

```python
add_float_slider(tag, *args, remember_value=False, **kwargs)
```

Add a float slider widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L242"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_float_text`

```python
add_float_text(tag, *args, remember_value=False, **kwargs)
```

Add a float text widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L173"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_int_slider`

```python
add_int_slider(tag, *args, remember_value=False, **kwargs)
```

Add a integer slider widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L225"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_int_text`

```python
add_int_text(tag, *args, remember_value=False, **kwargs)
```

Add a integer text widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L103"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_label`

```python
add_label(*args, **kwargs)
```

Add a label widget to the container. 



**Args:**
 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L129"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_text`

```python
add_text(tag, *args, remember_value=False, **kwargs)
```

Add a text widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 



**Example:**
 The following example demonstrates how to add a text widget to the GUI: 

``` gui = EasyGUI()```
    >>> gui.add_text("text", "Enter some text:")
    >>> gui.show()


---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L153"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `add_textarea`

```python
add_textarea(tag, *args, remember_value=False, **kwargs)
```

Add a textarea widget to the container. 



**Args:**
 
 - <b>`tag`</b> (str):  The tag to identify the widget. 
 - <b>`args`</b>:  Args for the widget. 
 - <b>`remember_value`</b> (bool):  Remember the last value. 
 - <b>`kwargs`</b>:  Kwargs for the widget. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L321"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `clear`

```python
clear()
```

Clear the widgets in the container. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L305"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `restore_default_settings`

```python
restore_default_settings()
```

Restore the default settings and clear the widgets. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L293"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `save_settings`

```python
save_settings()
```

Save the widget values to the configuration file. 

---

<a href="../easy_gui_jupyter/easy_gui_jupyter.py#L313"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>method</kbd> `show`

```python
show()
```

Show the widgets in the container. 




---

_This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
