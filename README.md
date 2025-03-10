# Get Papers List

A Python program to fetch research papers from PubMed and filter those with at least one author affiliated with a pharmaceutical or biotech company.

---

## **Features**

- Fetches research papers from PubMed using a search query.
- Filters papers based on author affiliation with pharmaceutical or biotech companies.
- Extracts relevant details, including emails of authors when available.
- Outputs results in a CSV format for easy viewing and analysis.

---

## **How the Code is Organized**

The program is organized into the following components:

### 1. **`get_papers.py`**
   - The main script that fetches papers from PubMed, filters them, and outputs the results.
   - Contains functions for:
     - **Fetching Paper IDs**: `fetch_paper_ids()`
     - **Fetching Paper Details**: `fetch_paper_details()`
     - **Checking Pharmaceutical/Biotech Affiliations**: `is_pharma_biotech()`
     - **Extracting Emails**: `extract_email()`

### 2. **Command-Line Interface**
   - The program is executed via the command line using `poetry run get-papers-list`.
   - Supports the following options:
     - `query`: The PubMed query to search for papers.
     - `-d` or `--debug`: Enables debug mode.
     - `-f` or `--file`: Saves the results to a CSV file.

### 3. **Dependencies**
   - The program uses the following libraries:
     - `requests`: For making HTTP requests to the PubMed API.
     - `lxml`: For parsing XML responses from PubMed.
     - `pandas`: For creating and saving the results as a CSV file.

---

## **Installation and Execution**

### **Prerequisites**
- Python 3.8 or higher.
- Poetry (for dependency management).

### **Installation Steps**
1. **Clone the repository:**
   ```bash
   git clone https://github.com/sanjudev1/get-papers-list.git
   cd get-papers-list
