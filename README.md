# create-calculator-using-tkinter-
Tkinter is the Python interface to the Tk GUI toolkit shipped with Python.

While creating any GUI Application there are mainly two steps:

The first step is to create a User Interface.

The second step is the most important one and in this, to add functionalities to the GUI

Now let's begin with creating a simple calculator app using Tkinter in Python which is used for basic arithmetic calculations.




Import Tkinter

    from tkinter import *

create a main window

     root=Tk()

Adding a name of the window
     
    root.title("simple Calculator")
    
    
#Calculator App Code


           root=Tk()
           root.title("simple Calculator")
           #define function
           def button_click(number):
               current=e.get()
               e.delete(0,END)
               e.insert(0,str(current) +str(number))
           def button_clear():
               e.delete(0,END)
           def button_add():
               global operator
               operator="Addition"
               frist=e.get()
               global f_num
               f_num=int(frist)
               e.delete(0,END)
           def button_sub():
               global operator
               operator="Subtraction"
               frist=e.get()
               global f_num
               f_num=int(frist)
               e.delete(0,END)
           def button_mul():
               global operator
               operator="Multiplication"
               frist=e.get()
               global f_num
               f_num=int(frist)
               e.delete(0,END)
           def button_div():
               global operator
               operator="Division"
               frist=e.get()
               global f_num
               f_num=int(frist)
               e.delete(0,END)
           def button_equal():
               second=e.get()
               e.delete(0,END)
               if operator=="Addition":
                   e.insert(0,f_num+int(second))
               if operator=="Subtraction":
                   e.insert(0,f_num-int(second))
               if operator=="Multiplication":
                   e.insert(0,f_num*int(second))
               if operator=="Division":
                   e.insert(0,f_num/int(second))
           e=Entry(root,width=35,fg="black",bg="white",borderwidth=5)
           e.grid(row=0,column=0,columnspan=3,padx=10,pady=10)
           #Button declaration
           button0=Button(root,text="0",padx=5,pady=10,command=lambda:button_click(0))
           button1=Button(root,text="1",padx=5,pady=10,command=lambda:button_click(1))
           button2=Button(root,text="2",padx=5,pady=10,command=lambda:button_click(2))
           button3=Button(root,text="3",padx=5,pady=10,command=lambda:button_click(3))
           button4=Button(root,text="4",padx=5,pady=10,command=lambda:button_click(4))
           button5=Button(root,text="5",padx=5,pady=10,command=lambda:button_click(5))
           button6=Button(root,text="6",padx=5,pady=10,command=lambda:button_click(6))
           button7=Button(root,text="7",padx=5,pady=10,command=lambda:button_click(7))
           button8=Button(root,text="8",padx=5,pady=10,command=lambda:button_click(8))
           button9=Button(root,text="9",padx=5,pady=10,command=lambda:button_click(9))
           button10=Button(root,text="+",padx=5,pady=10,command=lambda:button_add())
           button11=Button(root,text="-",padx=5,pady=10,command=lambda:button_sub())
           button12=Button(root,text="*",padx=5,pady=10,command=lambda:button_mul())
           button13=Button(root,text="/",padx=5,pady=10,command=lambda:button_div())
           button14=Button(root,text="=",padx=5,pady=10,command=lambda:button_equal())
           button15=Button(root,text="clear",padx=20,pady=10,command=lambda:button_clear())
           #Button positon
           button0.grid(row=4,column=0)
           button1.grid(row=1,column=0)
           button2.grid(row=1,column=1)
           button3.grid(row=1,column=2)
           button4.grid(row=2,column=0)
           button5.grid(row=2,column=1)
           button6.grid(row=2,column=2)
           button7.grid(row=3,column=0)
           button8.grid(row=3,column=1)
           button9.grid(row=3,column=2)
           button10.grid(row=1,column=3)
           button11.grid(row=2,column=3)
           button12.grid(row=3,column=3)
           button13.grid(row=4,column=2)
           button14.grid(row=4,column=1)
           button15.grid(row=4,column=3)
           root.mainloop()
           
    
              
