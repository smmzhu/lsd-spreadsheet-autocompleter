# README

The purpose of this script is give it an `input.csv` with names and be able to fill out the rest of the information such as email and phone number. This Python script reads data from a Google Sheets document using the `gspread` library and the Google Drive API, and then creates a `Pandas` DataFrame to organize the data. The script then defines a class `Student`, which takes the rows of the `Pandas` DataFrame as input and parses them into individual attributes of a student object. Finally, the script provides a method for accessing each attribute of a student object based on a given parameter, then outputs all the information onto an `output.csv` file.

## Prerequisites

Before running this script, the following libraries must be installed:

- pandas
- gspread
- oauth2client
- google-auth

Also, to authenticate with the Google Drive API, the script requires a JSON file with Google Drive API credentials.

## Usage

The script is meant to be run in a Google Colab notebook or a local Python environment with the necessary libraries installed. After importing the required libraries and authenticating with the Google Drive API, the script reads data from a Google Sheets (the current example is LSD Contact Info Sheet 21-22) and converts it to a Pandas DataFrame.

The user can then modify the list of attributes that they want the code to look up in the Google Sheet and add to the Pandas DataFrame. 

## Parameters

The current parameters of a student object (and the columns of the example Google Sheet) are:

- first name
- pref first name
- last name
- grade
- period
- level
- phone
- email
- address
- p1name (parent 1 name)
- p1email (parent 1 email)
- p1phone (parent 1 phone)
- p2name (parent 2 name)
- p2email (parent 2 email)
- p2phone (parent 2 phone)
