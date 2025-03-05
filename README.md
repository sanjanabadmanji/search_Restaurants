# search_Restaurants

# README

## Overview
This Python script automates the process of retrieving the **top 10 restaurants** in a specified city using **Google Maps**. It extracts key details such as:
- **Restaurant Name**
- **Rating**
- **Reviews**

The collected data is stored in a **JSON file** for easy access.

## Prerequisites
Ensure you have the following installed:
- **Python**
- **Selenium WebDriver**
- **WebDriver Manager**

## Installation

1. Clone this repository or download the script.
2. Install the required dependencies using:
   ```sh
   pip install selenium webdriver-manager
   ```

## How It Works
1. **User Input:** Prompts the user to enter a city name.
2. **Google Maps Search:** Automates a search for "top restaurants in {city}".
3. **Scrolling & Data Extraction:** Scrolls through results and collects restaurant details.
4. **JSON Storage:** Saves extracted details into a JSON file.

## Usage
Run the script using:
```sh
python script_name.py
```
Replace `script_name.py` with the actual script filename.

### Example
**Input:**
```
Enter the name of a city: New York
```

**Output:**
```
Total restaurants found: 12
name_element: Lotus Pavilion, ITC Gardenia - Restaurants In Bengaluru, rating_element: 4.5, reviews_element: (2,993)
name_element: Shiro, rating_element: 4.4, reviews_element: (4,978)
name_element: Spice Terrace, rating_element: 4.3, reviews_element: (2,056)
```

## JSON Output Format
The script generates a JSON file with the following format:
```json
{
    "Lotus Pavilion, ITC Gardenia - Restaurants In Bengaluru": {
        "rating": "4.5",
        "reviews": "(2,993)"
    },
    "Shiro": {
        "rating": "4.4",
        "reviews": "(4,978)"
    },
    "Spice Terrace": {
        "rating": "4.3",
        "reviews": "(2,056)"
    },
    "Time Traveller (Urban Herbivore)": {
        "rating": "4.3",
        "reviews": "(2,909)"
    },
    "Le Cirque Signature": {
        "rating": "4.5",
        "reviews": "(718)"
    },
    "The Only Place": {
        "rating": "4.2",
        "reviews": "(8,063)"
    },
    "The Raj Pavillion": {
        "rating": "4.5",
        "reviews": "(399)"
    },
    "Mangalore Pearl": {
        "rating": "4.4",
        "reviews": "(4,889)"
    },
    "Karavalli": {
        "rating": "4.5",
        "reviews": "(3,879)"
    },
    "Blue Terrain": {
        "rating": "4.5",
        "reviews": "(626)"
    }
}
```

## Troubleshoot
### 1. **Selenium WebDriver Not Found**
- Ensure Edge WebDriver is installed.
- Update WebDriver using:
  ```sh
  pip install --upgrade webdriver-manager
  ```

### 2. **No Restaurants Found**
- Check the internet connection.
- Increase the scroll limit to load more results.

## Author
- **Sanjana Badmanji**
- **Contact:** sanjanabadmanji@gmail.com


