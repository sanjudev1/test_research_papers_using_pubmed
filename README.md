# Get Papers List

A Python program to fetch research papers from PubMed and filter those with at least one author affiliated with a pharmaceutical or biotech company.

---

## **How the Code is Organized**

The program is organized into the following components:

1. **`get_papers.py`**:
   - The main script that fetches papers from PubMed, filters them, and outputs the results.
   - Contains functions for:
     - Fetching paper IDs (`fetch_paper_ids`).
     - Fetching paper details (`fetch_paper_details`).
     - Checking for pharmaceutical/biotech affiliations (`is_pharma_biotech`).
     - Extracting email addresses (`extract_email`).

2. **Command-Line Interface**:
   - The program is executed via the command line using `poetry run get-papers-list`.
   - Supports the following options:
     - `query`: The PubMed query to search for papers.
     - `-d` or `--debug`: Enables debug mode.
     - `-f` or `--file`: Saves the results to a CSV file.

3. **Dependencies**:
   - The program uses the following libraries:
     - `requests`: For making HTTP requests to the PubMed API.
     - `lxml`: For parsing XML responses from PubMed.
     - `pandas`: For creating and saving the results as a CSV file.

---

## **Installation and Execution**

### **Prerequisites**
- Python 3.8 or higher.
- Poetry (for dependency management).

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/sanjudev1/get-papers-list.git
   cd get-papers-list


---

## **Step 2: Code Organization and Modularization**

To break the program into a module and a command-line program:

1. **Create a Module**:
   - Move the core functionality (e.g., `fetch_paper_ids`, `fetch_paper_details`, etc.) into a separate module file, e.g., `pubmed_tools.py`.

2. **Update the Command-Line Script**:
   - Import the module in `get_papers.py` and use its functions.
#   t e s t _ r e s e a r c h _ p a p e r s _ u s i n g _ p u b m e d  
 