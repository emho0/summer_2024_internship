# summer_2024_internship
Python notebooks coded mainly on Google Colab for an internship.

Quebec national library scraper - script for a headless webscraper to collect texts from the digital library for the corpus.

Segementation - Part of data processing to prepare the corpus for Topic Modeling.

Topic modeling notebook - code for topic modeling using BERTopic. Precalculation of the embeddings was done, as repeatedly calculating embeddings would be an extremely time consuming process. Due to scale of corpus (over 1000 texts), a manual entry of batches of text was required, hence the lack of iteration through the batches. The model used is from huggingface.

NER - Named entity recognition to recognize place names using Flair model. Again, it is intentional that the code does not iterate over batches due to the scale of the corpus. Running code manually was the best way to ensure that all data was saved / no output was lost or half-completed during the process, as crashes due to lack of disk space, RAM, or gcolab runtime limits occurred multiple times.
