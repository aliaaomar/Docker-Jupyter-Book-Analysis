# Goodreads & Harry Potter Data Analysis (Dockerized)

A containerized Python data analysis environment exploring the Goodreads books dataset, featuring exploratory data analysis (EDA), missing value diagnostics, and targeted series analysis for the Harry Potter book franchise.

---

## Analysis Overview

* **Data Ingestion & Inspection:** Loads and evaluates Goodreads book catalog metadata from `books.csv`.
* **Data Cleaning & Quality Diagnostics:** Systematically inspects missing and null values across columns such as titles, authors, publication years, and ratings.
* **Harry Potter Series Deep Dive:** Filters and analyzes metrics for J.K. Rowling's Harry Potter series, including publication timeline, rating counts, and average user ratings.
* **Reproducible Execution:** Fully containerized using Docker to ensure dependency isolation and zero-configuration execution in Jupyter Notebook.

---

## Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Jupyter Notebook
* **Environment & Containerization:** Docker

---

## Project Structure

* `Dockerfile` — Builds the containerized Python and Jupyter data science environment
* `HarryPotter.ipynb` — Jupyter Notebook containing data preprocessing, cleaning, and EDA workflows
* `books.csv` — Goodreads dataset containing book metadata and rating statistics
* `requirements.txt` — Python dependencies for the analysis environment
* `cloudpdf.pdf` — Exported documentation and preview of the executed analysis

---

## Getting Started

### Prerequisites

* Docker Desktop installed and running.

---

### Installation & Run with Docker

1. **Clone the repository:**
   * `git clone https://github.com/aliaaomar/docker-jupyter-book-analysis.git`
   * `cd docker-jupyter-book-analysis`

2. **Build the Docker image:**
   * `docker build -t harry-potter-eda .`

3. **Run the container:**
   * `docker run -p 8888:8888 harry-potter-eda`

4. **Access Jupyter Notebook:**
   * Open your browser and navigate to the URL printed in your terminal output (typically `http://localhost:8888/?token=...`) to run `HarryPotter.ipynb`[cite: 1].

---

### Running Locally (Without Docker)

1. **Create and activate a virtual environment:**
   * `python -m venv venv`
   * `source venv/bin/activate` *(On Windows: `venv\Scripts\activate`)*

2. **Install dependencies:**
   * `pip install -r requirements.txt`

3. **Launch Jupyter Notebook:**
   * `jupyter notebook`
