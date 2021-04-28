# Example

#Editado por Geovani

import tkinter as tk

global clicked

clicked=False

def my_click():
    global clicked
    clicked=not clicked
    
    if clicked:
        check=tk.Label(text="Encendido")
    else:
        check=tk.Label(text="Apagado")
    
    check.grid(row=2, column=0)

window = tk.Tk()

greeting = tk.Label(text="Hello, Tkinter")

greeting.grid(row=0, column=0)

button=tk.Button(text="click me", width=25, height=3, command=my_click)
button.grid(row=1, column=0 )

check=tk.Label(text="Apagado")
check.grid(row=2, column=0)

window.mainloop()
