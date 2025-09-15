# KEN3140 – Webshop RDF & SPARQL Project

## Project Overview

This project models products from the Logitech webshop as RDF data and explores them through SPARQL queries.  
We started from a CSV dataset of approximately 80 Logitech products, transformed it into RDF (Turtle), and then wrote queries (A–G) to answer specific knowledge questions.  
The work involved data preparation, ontology design, RDF generation, and query formulation.

## Team Members

- **Nehir Sarihan**
- **Noam Favier**
- **Trinh Le**
- **Jinyang Wen**

## Work Distribution

### Nehir Sarihan

- Conducted data cleaning of the CSV file, ensuring consistent formatting of prices, attributes, and values.
- Assisted in defining schema design for products, categories, and brands.
- Documented the data transformation workflow.

### Noam Favier

- Implemented the Python/Jupyter pipeline to convert CSV into RDF (Turtle).
- Developed helper functions for URI handling and literal conversion.
- Implemented and validated SPARQL queries A–D, F, and G.
- Ensured consistent use of namespaces (`ex:`, `schema:`) and alignment with the ontology.

### Trinh Le

- Designed SPARQL queries and tested them against the RDF graph.
- Verified semantic correctness of query outputs (brand–category relations, product recommendations, average prices).
- Prepared query outputs and formatted results for the report.

### Jinyang Wen

- Implemented Query E, integrating external data from Wikidata (e.g., founder, headquarters, website).
- Supported integration of external knowledge into the documentation.
- Contributed to the final preparation of the README.

## Role of AI

Artificial Intelligence (ChatGPT) was used for:

- Formatting and structuring the Jupyter notebook and README.
- Assisting with debugging of Python and SPARQL code.
- Providing guidance on data transformation best practices.

All substantive work — dataset cleaning, RDF modeling, SPARQL query design, and analysis — was carried out by the project members.

## Queries Implemented

- **Query A:** Categories and brand for a given item.
- **Query B:** Cross-category products sharing the same brand.
- **Query C:** Average price and rating grouped by brand.
- **Query D:** Products in a category sorted by average brand price.
- **Query E:** External enrichment from Wikidata (headquarters, founder, etc.).
- **Query F:** Similar products based on brand/category overlap.
- **Query G:** Custom query — find mice under $100 with rating above 4.0.

## How to Run

1. Open the Jupyter Notebook (`webshop.ipynb`) or the Python script (`webshop.py`).
2. Load the cleaned CSV dataset.
3. Run all cells to generate the Turtle file (`webshop.ttl`).
4. Execute the queries in the notebook to reproduce results.
5. For Query E, copy the Wikidata query into the [Wikidata Query Service](https://query.wikidata.org/).

## Deliverables

- Cleaned **CSV dataset**
- **Turtle (TTL)** RDF file
- **Jupyter Notebook (.ipynb)** with transformation and queries
- **README.md** (this file) documenting contributions and methodology
