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

Usage
Run the script to fetch Pokémon data, process it, and store it in Google Cloud Storage and BigQuery:

python pokemon_stat_checker.py
Check the BigQuery tables created with the fetched Pokémon data.

Google Cloud Configuration
Set up a Google Cloud Storage bucket and obtain the necessary credentials.

Create a BigQuery dataset and tables to store the Pokémon data.

Replace the placeholder values in the script with your actual Google Cloud Storage and BigQuery information.

BigQuery Setup
The script creates the following tables in BigQuery:

EntityTable
TypeTable
AbilityTable
FactTable
Ensure that the schema definitions in the script match your data structure.

### Prerequisites

Before running the script, you need to have the following:

- Python 3.x
- Google Cloud Storage account
- Google Cloud Platform project with BigQuery enabled

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JustinDavid2g/Pokémon-stat-checker-.git

   
