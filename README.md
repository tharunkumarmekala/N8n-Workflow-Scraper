# N8n Workflow Scraper with Google Drive and Google Sheets Integration

This project provides a Python script to automate the scraping of n8n workflows from a given URL, extract their JSON data and metadata, save the JSON files locally, upload them to Google Drive, and update a Google Sheet with the extracted information and the Google Drive links.

It also includes a Gradio interface for easy execution of the scraping process.

## Features

*   **Web Scraping**: Navigates to a specified n8n workflow search results page and extracts links to individual workflows.
*   **Pagination Handling**: Clicks the "Load more templates" button to retrieve links from multiple pages.
*   **Data Extraction**: Extracts workflow JSON, title, description, and URL from each workflow page.
*   **Local Storage**: Saves the extracted workflow JSON data as individual `.json` files locally.
*   **Google Drive Integration**: Uploads the local JSON files to a specified Google Drive folder and makes them shareable.
*   **Google Sheets Integration**: Appends workflow metadata (title, description, URL, JSON filename, and Drive link) to a specified Google Sheet.
*   **Gradio Interface**: Provides a user-friendly web interface to input the required parameters and run the scraping process.

## Prerequisites

*   Python 3.7+
*   Google Cloud Project with Google Drive and Google Sheets APIs enabled.
*   Credentials for Google API authentication (handled by Google Colab's `auth.authenticate_user()`).
*   A Google Sheet to store the workflow data.
*   A Google Drive folder to store the workflow JSON files.
> ⚙️ **Note**: This automation is compatible with [n8n workflows](https://n8n.io/workflows/), allowing seamless integration into modular automation pipelines.

## Setup

1.  **Open in Google Colab**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tharunkumarmekala/N8n-Workflow-Scraper/blob/main/N8N_Automation.ipynb) Open this notebook in Google Colab.
2.  **Install Dependencies**: Run the first code cell to install the required libraries:
