# Pokémon Stat Checker

This project is a Pokémon stat checker that fetches data from the PokeAPI, processes it, and stores it in Google Cloud Storage and BigQuery.

## Overview

The Pokémon Stat Checker is a Python script that interacts with the [PokeAPI](https://pokeapi.co/) to fetch information about Pokémon. The fetched data is processed, stored in a CSV file, uploaded to Google Cloud Storage, and then loaded into BigQuery tables.

## Getting Started
Install the required Python packages:

1. os
2. io
3. from google.cloud import storage
4. from google.oauth2 import service_account

## ELT Process
![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/759160ad-2435-43af-a524-751f16179b3a)

   ### Extract
     The Extracts proccess of this code gathers 

python pokemon_stat_checker.py
Check the BigQuery tables created with the fetched Pokémon data.

Google Cloud Configuration
Set up a Google Cloud Storage bucket and obtain the necessary credentials.

Create a BigQuery dataset and tables to store the Pokémon data.

Replace the placeholder values in the script with your actual Google Cloud Storage and BigQuery information.

BigQuery Setup
The script creates the following tables in BigQuery:

1. EntityTable
2. TypeTable
3. AbilityTable
4. FactTable

Here is a visiual representation: 
![image](https://github.com/JustinDavid2g/Pok-mon-stat-checker-/assets/121201630/8f36c506-963e-4885-becf-b4e0a9f21fc5)

Ensure that the schema definitions in the script match your data structure.

## Prerequisites

Before running the script, you need to have the following:

- Python 3.x
- Google Cloud Storage account
- Google Cloud Platform project with BigQuery enabled


   
