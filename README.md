# Exploring Airbnb Market Trends in New York City

![NYC Skyline](https://images.unsplash.com/photo-1448317846460-907988886b33?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

*Photo by [Todd Quackenbush](https://unsplash.com/@toddquackenbush) on [Unsplash](https://unsplash.com)*

## Project Overview

This project delves into the vibrant New York City Airbnb market, exploring various trends in room types, neighborhood distribution, pricing, and more. By merging datasets from different file formats such as `.csv`, `.tsv`, and `.xlsx`, this project aims to provide insights that could be valuable for real estate professionals, travelers, and data enthusiasts alike.

## Motivation

With New York City being one of the most popular tourist destinations globally, the demand for temporary lodging is immense. Airbnb, as a key player in this market, offers diverse listings ranging from shared rooms to entire homes. This project seeks to uncover patterns and trends within this market, focusing on the most common room types, price distributions, and neighborhood prevalence.

## Data Sources

The analysis is based on data from 2019, comprising the following files:

- **`airbnb_price.csv`**: Contains data on Airbnb listing prices and locations.

  - **`listing_id`**: Unique identifier of the listing.

  - **`price`**: Nightly listing price in USD.

  - **`nbhood_full`**: Name of the borough and neighborhood where the listing is located.

- **`airbnb_room_type.xlsx`**: Contains data on Airbnb listing descriptions and room types.

  - **`listing_id`**: Unique identifier of the listing.

  - **`description`**: Listing description.

  - **`room_type`**: Room types including shared rooms, private rooms, and entire homes/apartments.

- **`airbnb_last_review.tsv`**: Contains data on Airbnb host names and review dates.

  - **`listing_id`**: Unique identifier of the listing.

  - **`host_name`**: Name of the listing host.

  - **`last_review`**: Date when the listing was last reviewed.

## Analysis Plan

1. **Data Cleaning:**

   - Load and clean the datasets (`airbnb_last_review.tsv`, `airbnb_price.csv`, `airbnb_room_type.xlsx`).

   - Address any discrepancies in room types using string similarity techniques.

2. **Analysis Questions:**

	-	What is the most common room type in Airbnb listings for NYC?

	-	Which boroughs do Airbnb listings exist in and which one is the most prevalent?

	-	What is the average price for each room type and borough combination?

	-	What is the price distribution for each room type?

	-	Which neighborhoods have the most Airbnb listings?

## Analysis Results 

- **Room Type Distribution**: The most common room type is **entire home/apt** with around 13,000 listings, followed by **private rooms** ($\approx$ 11,000 listings), and **shared rooms** ($\approx$ 500 listings).

![Room Type Distribution](https://github.com/MohamedMostafa259/ExploringAirbnbMarketTrends/blob/2d668c93c0a4629001c686877aa078095a8e1a92/visualizations/Frequency%20of%20each%20Room%20Type.png)

<br>

---

<br>

- **Borough Distribution**: Airbnb listings are most prevalent in **Brooklyn** and **Manhattan** ($\approx$ 10,500 listings each), followed by **Queens** ($\approx$ 3,500 listings), **Bronx** ($\approx$ 700 listings), and **Staten Island** ($\approx$ 250 listings).

![Borough Distribution](https://github.com/MohamedMostafa259/ExploringAirbnbMarketTrends/blob/2d668c93c0a4629001c686877aa078095a8e1a92/visualizations/Frequency%20of%20each%20Borough.png)

<br>

---

<br>

- **Average Price by Room Type**:

  - **Entire home/apt**: $\approx$ $195/night

  - **Private room**: $\approx$ $80/night

  - **Shared room**: $\approx$ $50/night

  - **Note:** However the average price of shared rooms in Manhattan is higher than the average prices of those private rooms in the remaining boroughs.

    - **Average Price by Borough**:

        - **Manhattan**: $185/night

        - **Brooklyn**: $120/night

        - **Queens**: $90/night

![Average Price by Room Type and Borough](https://github.com/MohamedMostafa259/ExploringAirbnbMarketTrends/blob/2d668c93c0a4629001c686877aa078095a8e1a92/visualizations/The%20Average%20Price%20for%20each%20Room%20Type%20and%20Borough%20Combination.png)

<br>

---

<br>

- **Top Neighborhoods**: The most common neighborhoods include Bedford-Stuyvesant, Williamsburg, Harlem, and Bushwick, among others.

![Top Neighborhoods](https://github.com/MohamedMostafa259/ExploringAirbnbMarketTrends/blob/2d668c93c0a4629001c686877aa078095a8e1a92/visualizations/Frequency%20of%20the%20most%20common%2010%20neighborhoods.png)