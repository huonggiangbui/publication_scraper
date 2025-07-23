# publication_scraper
Web Scraping Publications & BERT inclusion/exclusion for systematic reviews of Generative AI papers with regard to social and educational impact. The results is then being used to conduct a thematic analysis.

RQ: Is it possible to automate systematic review of Generative AI papers in the field of computing education?

Method:
1. Scrape publications from popular databases (Semantic Scholar, DBLP, Web of Science, Google Scholar) based on keywords related to RQ & year range. Remove duplicates papers based on title and abstract and DOI (`search-and-clean.ipynb`)
2. Get metadata for the scraped papers (title, abstract, authors, year, venue, etc.) and save them to a CSV file (`get-paper-metadata.ipynb`)
3. Snowball relevant papers to find more related publications (`snowballing.ipynb`)
4. Use BERT to classify papers as relevant or not relevant to the systematic review (`bert-classification.ipynb`)
5. Conduct thematic analysis on the relevant papers

Script originally written by Harry Ye (UofT) and Giang Bui (UofT). Adapted from the original script by Giang Bui. Project supervised by Dr. Michael Liut (UofT) and Dr. Tingting Zhu (UofT). This project is funded by SSHRC Grant 2023-2024.
