"# Basic-Python-Calculator" 
from tkinter import *

window=Tk()
window.geometry("400x600")
window.title("Calculator")

label_1=Label(window,text="Fist Number",font=("Calibri",25))
label_1.pack()

txt1=Text(window,height=2,width=20,font=("Calibri",25))
txt1.pack()

label_2=Label(window,text="Second Number",font=("Calibri",25))
label_2.pack()

txt2=Text(window,height=2,width=20,font=("Calibri",25))
txt2.pack()

def add():
   n1=int(txt1.get("1.0","end-1c"))
   n2=int(txt2.get("1.0","end-1c"))
   print(n1+n2)

def sub():
   n1=int(txt1.get("1.0","end-1c"))
   n2=int(txt2.get("1.0","end-1c"))
   print(n1-n2)

def mul():
   n1=int(txt1.get("1.0","end-1c"))
   n2=int(txt2.get("1.0","end-1c"))
   print(n1*n2)

def dev():
   n1=int(txt1.get("1.0","end-1c"))
   n2=int(txt2.get("1.0","end-1c"))
   print(n1/n2)

btn1=Button(window,text="Addition",command=add,font=("Calibri",30))
btn1.pack()
btn2=Button(window,text="Subtraction",command=sub,font=("Calibri",30))
btn2.pack()
btn3=Button(window,text="Multipication",command=mul,font=("Calibri",30))
btn3.pack()
btn4=Button(window,text="Division",command=dev,font=("Calibri",30))
btn4.pack()


window.mainloop()

