# DOCS_SIMILARITY — Backend

A Java Spring Boot backend that analyzes documents and identifies common word sequences using Data Structures and Algorithms.

## Features
- Supports TXT, PDF, and DOCX files.
- Extracts and tokenizes document text.
- Identifies common word sequences using a Generalized Suffix Array.
- Uses the Kasai LCP algorithm to find common prefixes.
- Calculates similarity scores and ranks document pairs.
- Includes unit and integration tests.

## Processing Flow

```mermaid
flowchart TD
    A[Upload Documents] --> B[Extract Text]
    B --> C[Tokenize Words]
    C --> D[Build Generalized Suffix Array]
    D --> E[Calculate LCP using Kasai]
    E --> F[Find Common Word Sequences]
    F --> G[Merge Overlapping Matches]
    G --> H[Calculate Similarity Scores]
    H --> I[Rank Document Pairs]
./mvnw spring-boot:run
