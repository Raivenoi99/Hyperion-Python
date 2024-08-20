### Custom Python-Like Scripting Language for GUI Applications

This project introduces a new Python-inspired scripting language designed for creating graphical user interfaces (GUIs) using Tkinter. The language syntax aims to simplify the process of building GUIs while maintaining the readability and ease of Python.

#### Key Features:
- **Simplified Window Creation**: Initialize and customize windows with straightforward commands.
- **Custom Print Functionality**: Use a unique `printfunc` syntax for outputting text to the console.
- **GUI Components**: Easily create and position frames and other Tkinter widgets with custom properties.
- **Delayed Execution**: Incorporate delays in execution with a custom `system.sleep` function, leveraging Tkinter's event loop.
- **User Input Dialogs**: Simplified syntax for creating input dialogs.

#### Example Script:
```python
import tkinter as tk

Root = tk.Tk()
Root.Title("Gui")

frame = tk.Frame(Root, bg="#ff00ff", bd=5)
frame.place(x=10, y=10)

printfunc = lambda text: print(text)
printfunc("Hello, World!")
Root.after(2000, lambda: printfunc("Hello, World!"))

input_value = tk.simpledialog.askstring("Input", "This is input")

Root.mainloop()
```

This project is ideal for developers interested in experimenting with new scripting paradigms or those who want to create simple GUIs with a Pythonic yet distinct syntax.
