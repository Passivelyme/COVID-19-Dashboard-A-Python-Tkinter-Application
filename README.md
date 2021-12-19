# Representing data using tkinter

This is a simple introduction to use the code in any way to represent data in gui from using python's inbuilt function tkinter from a csv file VS Code.

Things you'll need:

* [Python](https://www.python.org/downloads/)
* [pip](https://pypi.org/project/pip/)
* pandas package
  >pip install pandas
* Rest of the packages are inbuilt so no worries.

## Functions ins the code

>def restart_program():
  
  This function is to restart the whole tkinter window

>def submit():

This function is main as in this we take the input from the user and use the tkinter entry command to use the user input data for searching the specific data in the csv files.

>def iget():

This function is to trigger the command
>n_but=Button(main_root,text = 'Next', command =iget)

as this command will call the function and it will act as a enter key in the tkinter window.

## Csv files

states.csv and state_wise.csv are used in the code

>These csv files are taken from the gov site [Csv file](https://data.covid19india.org/)

# Rough idea of the GUI

In the code we basically use the concept of if else and for loop.

* first the user is provided with two options of how the data is to be represented.

>Display the data as Date wise

>Display the data as State wise

* Then the user is supposed to enter 1 or 2 according to the choice.
* if the choice is 1 the the date that can be entered is
 between 30-10-2020 to 01-10-2021 and press next.
* If the choice is 2 the just state name has to be entered with th first letter in capslock on and press next.
* If by any chance the users need to start over he can just press the refresh button 
* The refresh button only appears when the choice 1-2 is entered.

## #All the data taken are from the csv file and according to government site, the csv contain data till First October,2021
