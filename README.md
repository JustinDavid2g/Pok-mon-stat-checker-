# Pokémon Stat Checker

This project is a Pokémon stat checker that fetches data from the PokeAPI, processes it, and stores it in Google Cloud Storage and BigQuery.

## What is this?

The Pokémon Stat Checker is a Python script that interacts with the [PokeAPI](https://pokeapi.co/) to fetch information about Pokémon. The fetched data is processed, stored in a CSV file, uploaded to Google Cloud Storage, and then loaded into BigQuery tables.

## Getting Started
Install the required Python packages:

* os
* io
* import google.cloud import storage
* import google.oauth2 import service_account
* import requests
* import pandas as pd

## ELT Process
![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/b5acf62f-570a-450d-82eb-abe8fb5489e9)



   ## Extract
   The Extraction proccess of this code gathers the Data from the pokemon API website, filters it, and then 
   transforms it into a readable CSV file.

   The CSV File:
   
   ![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/7035337e-a95a-4355-a68e-c14c98cbb1f3)



   ## Load 
   This part of the code handles loading the CSV into your google cloud storage.
   You will need to set up a Google Cloud Storage bucket and obtain the necessary credentials in order for this part of 
   the code to work
   ![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/ccd1fc6d-6e7a-49b5-be87-521eb4b7ce2a)


   ## Transform
   The next part of the code is supposed to be a script that takes the CSV file and uses it to set up and transforms the data into tables.

BigQuery Setup
The script creates the following tables in BigQuery:

*   EntityTable
*   TypeTable
*   AbilityTable
*   FactTable

Here is a visiual representation: 
![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/8f36c506-963e-4885-becf-b4e0a9f21fc5)

Ensure that the schema definitions in the script match your data structure.
After this your should be able to upload your tables from BigQuery to Looker Studio and precede 
with your visualization.

## Data
   These are some data charts I was able to construct on Looker Studio using the data gathered,   
   ![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/cfe83eac-ce7d-4db3-90a6-adf2607d41fe)



## Prerequisites

Before running the script, you need to have the following:

- Python 
- Google Cloud Storage account
     * your credientials and bucket name
- Google Cloud Platform project with BigQuery along
     with the necessary roles enabled such as:
     * BigQuery Data Editor
     * BigQuery Job User
     * Storage Admin


   
