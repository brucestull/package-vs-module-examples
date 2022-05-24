# Example Python Interpreter Commands

1. Start python shell:  
    `python`
    ```
    PS C:\Users\User\Programming\package-vs-module-examples\basic_example> python
    Python 3.10.3 (tags/v3.10.3:a342a49, Mar 16 2022, 13:07:40) [MSC v.1929 64 bit (AMD64)] on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    ```

1. Import the module:  
    `import basic_python_module`  
    ```
    >>> import basic_python_module
    >>>
    ```

1. Try typing some stuff in interpreter:  
    * `basic_python_module`  
        ```
        >>> basic_python_module
        <module 'basic_python_module' from 'C:\\Users\\User\\Programming\\package-vs-module-examples\\basic_example\\basic_python_module.py'>
        >>>
        ```
    * `dir(basic_python_module)`  
        ```
        >>> dir(basic_python_module)
        ['__builtins__', '__cached__', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__', 'l', 's', 'TheClass', 'the_function']
        >>>
        ```
    * `basic_python_module.s`  
        ```
        >>> basic_python_module.s
        'One tequila, two tequila, three tequila floor!'
        >>>
        ```
    * `basic_python_module.l`  
        ```
        >>> basic_python_module.l
        ['a', 2, 'c']
        >>>
        ```
    * `basic_python_module.the_function(s)`  
        ```
        >>> basic_python_module.the_function(s)
        Traceback (most recent call last):
        File "<stdin>", line 1, in <module>
        NameError: name 's' is not defined
        >>>
        ```
    * `basic_python_module.the_function(basic_python_module.s)`  
        ```
        >>> basic_python_module.the_function(basic_python_module.s)
        The Argument: One tequila, two tequila, three tequila floor!
        >>>
        ```
    * `TheClass`  
        ```
        Traceback (most recent call last):
        File "<stdin>", line 1, in <module>
        NameError: name 'TheClass' is not defined
        >>>
        ```
    * `basic_python_module.TheClass`  
        ```
        >>> basic_python_module.TheClass
        <class 'basic_python_module.TheClass'>
        >>>
        ```
    * `basic_python_module.TheClass()`  
        ```
        >>> basic_python_module.TheClass()
        <basic_python_module.TheClass object at 0x0000014ED988E740>
        >>>
        ```
    * `c = basic_python_module.TheClass()`  
        ```
        >>> c = basic_python_module.TheClass()
        >>>
        ```
    * `c`  
        ```
        >>> c = basic_python_module.TheClass()
        >>> c
        <basic_python_module.TheClass object at 0x0000014ED988FEE0>
        >>>
        ```

1. Quit the Python interpreter:  
`quit()`
