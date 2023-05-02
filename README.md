# MUN Research Engine
A web application that allows users to search for news articles, academic papers, and UN documents based on a given agenda. It also provides information on a country's capital, region, and income level based on the ISO 2-letter code of the country name entered by the user.

## Usage
- Clone the repository
- Open index.html in your web browser / Alternatively, access the website from https://munresearch.github.io
- Enter your agenda and country name in the form and click the "Search" button

The website will retrieve the top 6 search results from different sources and display them in the table. It will also retrieve information about the country and display it in the table.

## APIs Used
- Google Search API
- World Bank API
- Datahub.io

## Technologies Used
- HTML
- CSS
- JavaScript

## Functions
- <b>search()</b>: This function is called when the form is submitted. It fetches search results using the Google Search API for news articles, academic papers, and UN documents based on the prompt entered by the user. It also fetches the ISO 2-letter code for the country entered by the user and uses it to retrieve information on the country's capital, region, and income level from the World Bank API. The search results and country information are then displayed in the table.
- <b>toTitleCase(string)</b>: This function takes a string and returns it in title case format, i.e., the first letter of each word is capitalized. This function exists to build the flag emoji. The flag emoji in the code is built using two Unicode regional indicator symbols, which are represented by two letters of the ISO 2-letter code of that country. These two symbols are then concatenated together and interpreted by emoji rendering engines as a flag emoji.
