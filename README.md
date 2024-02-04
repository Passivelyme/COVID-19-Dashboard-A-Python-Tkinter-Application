 ### COVID-19 Dashboard: A Python Tkinter Application

This repository contains the code for a COVID-19 dashboard application developed using Python and the Tkinter library. The application provides a user-friendly interface for viewing COVID-19 data in two different ways: date-wise and state-wise.

#### Prerequisites

To run this application, you will need the following:

- Python 3 or later
- Tkinter library (usually comes pre-installed with Python)
- Pandas library

#### Installation

To install the required libraries, open a terminal or command prompt and run the following commands:

```
pip install tkinter
pip install pandas
```

#### Running the Application

Once the required libraries are installed, you can run the application by following these steps:

1. Clone this repository to your local machine.
2. Open the `main.py` file in a text editor or IDE.
3. Make sure the Python interpreter is set to Python 3 or later.
4. Run the `main.py` file by clicking the "Run" button in your IDE or by using the following command in the terminal:

```
python main.py
```

#### User Interface

The application's user interface consists of the following elements:

- **Title:** "COVID-19 Dashboard"
- **Instruction:** "Covid-19 Data can be viewed in below two ways"
- **Options:**
  - "1- Display Data as Date wise"
  - "2- Display Data as State wise"
- **Choice Entry:** A text entry field for the user to enter their choice (1 or 2)
- **Submit Button:** A button to submit the user's choice
- **Output:** A text area that displays the COVID-19 data based on the user's choice

#### Code Explanation

The code for the application is organized into several functions:

- `restart_program()`: This function restarts the program when the "Refresh" button is clicked.
- `submit()`: This function is called when the user clicks the "Submit" button. It takes the user's choice and displays the COVID-19 data accordingly.
- `iget()`: This function is called when the user clicks the "Next" button after entering a date or state. It retrieves the data from the CSV files and displays it in the text area.

The main logic of the application is as follows:
