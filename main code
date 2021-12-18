import csv 
import os
import sys
from tkinter import *
from tkinter import font
import tkinter as tk
from tkinter import ttk
import pandas as pd
from pandas.core.frame import DataFrame
from tkinter import Label, Button
main_root =tk.Tk()
main_root.geometry("650x700")
def restart_program():
    python = sys.executable
    os.execl(python, python, * sys.argv)
def submit():
    k=int(Choice_entry.get())
    if(k==1):
        date_label =Label(main_root,text="Enter The Date").pack()
        date_input=Entry(main_root)
        date_input.pack()
        scrollbar = Scrollbar(main_root)
        scrollbar.pack(side=RIGHT,fill=Y)
        def iget():
            n=(date_input.get())            
            df = pd.read_csv('states.csv')
            k=df[df['Date']==n].index.values
            mylist = Text(main_root, yscrollcommand = scrollbar.set )
            for i in k:
                mylist.insert(END,df.loc[i].to_string())
                mylist.insert(END,"																				")
            mylist.pack(side=LEFT,fill=BOTH)
            scrollbar.config(command=mylist.yview)
        n_but=Button(main_root,text = 'Next', command =iget)
        n_but.pack()
        Button(main_root, text="Refresh", command=restart_program).pack()
    elif(k==2):
        State_label =Label(main_root,text="Enter The State").pack()
        State_name=Entry(main_root)
        State_name.pack()
        scrollbarv = Scrollbar(main_root,orient=VERTICAL)
        scrollbarv.pack(side=RIGHT,fill=Y)
        def iget():
            n=(State_name.get())
            df = pd.read_csv('state_wise.csv')
            k=df[df['State']==n].index.values
            mylist = Text(main_root, yscrollcommand = scrollbarv.set)
            mylist.pack()
            for i in k:
                mylist.insert(END,df.loc[i].to_string())
                mylist.insert(END,"																				")
            
            scrollbarv.config(command=mylist.yview)
        n_but=Button(main_root,text = 'Next', command =iget)
        n_but.pack()    
        Button(main_root, text="Refresh", command=restart_program).pack()
    else:
         Label.config(text="Invalid choice")  
main_root.title("Covid-19 Dashboard")
inf_label=Label(main_root, text="Covid-19 Dashboard",font=("Castellar Regular",18,)).pack()
Label_space=Label(main_root ).pack()
Label1=Label(main_root, text= "Covid-19 Data can be viewed in below two ways",font=(13)).pack()
Label2=Label(main_root, text= "1- Display Data as Date wise",font=(11)).pack()
Label3=Label(main_root, text= "2- Display Data as State wise",font=(11)).pack()
Label3=Label(main_root, ).pack()
Choice_label=Label(main_root,text = "Enter Your Choice",font=("calibre",10,"bold"))
Choice_label.pack()
Choice_entry=Entry(main_root,font=("calibre",10,))
Choice_entry.pack()
sub_btn=Button(main_root,text = 'Submit', command =submit).pack()
main_root.mainloop()
