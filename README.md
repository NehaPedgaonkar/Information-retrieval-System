# Information Retrieval System

## About

Implementation of an information extraction system that extracts structured information that is embedded in the natural language on webpages. Project uses the Google Custom Search API for the actual retrieval of results. 

This project implements two approaches to extract information (relations) from the web. The desired approach can be specified in the command line.

1. SpanBERT
2. GPT-3 API

Currently four types of relations are supported: **Schools_Attended, Work_for, Live_in,** and **Top_Member_Employees**.

# File Structure

```markdown
├── llm_ise
│   ├── lib
│   │   └── utils.py
├── main.py
├── EntityExtractor.py
├── QueryExecutor.py
└── SpanBertExtractor.py
├── README.md <-- You're here now!
└── setup.sh
```

| Filename                       | Description                                                                                     
|--------------------------------|----------------------------------------------------------------------------------------------------|
| `setup.sh`                     | Bash script for setting up environment                                                             |   
| `GPT3Extractor.py`             | Creates objects that process text using spaCy and extract using GPT3                               |
| `SpanBertExtractor.py`         | Creates objects that process text using spaCy and extract using spanBERT                           |
| `QueryExecutor.py`             | Creates class for query execution, response handling, and input processing                         |      
| `main.py`                      | Main function that handles the control flow                                                        | 
| `utils.py`                     | Utilities for processing documents + urls                                                          |
| `spacy_help_functions.py`      | Utilities for processing documents w/ spaCy                                                        |
|                                | sourced from [here](http://www.cs.columbia.edu/~gravano/cs6111/Proj2/spacy_help_functions.py)      |

