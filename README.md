# PROBLEM STATEMENT:
reating a Gen-AI agent that ingests real-time climate risk data and distills it into actionable insights for the insurance sector, especially aligned with frameworks like TNFD (Taskforce on Nature-related Financial Disclosures).

# SOP:
Real-time News Ingestion : Ingest news, ESG reports, scientific journals, regulatory updates.

Natural Language Processing (NLP) : Classify and summarize articles with a focus on:

                                  Climate risks (physical, transition), Biodiversity loss, Legal & regulatory changes, Regional exposure insights, 

Mapping to Insurance Impact:  Relate extracted insights to insurance products:, Property & casualty, Crop and agri-insurance, Reinsurance portfolios

Output Generation : 

            ┌────────────────────┐
            │  News/API Ingestor │◄───── Scheduled or streaming
            └────────┬───────────┘
                     │
        ┌────────────▼────────────┐
        │  Text Cleaner & Parser  │
        └────────────┬────────────┘
                     │
          ┌──────────▼──────────┐
          │ LLM (NLP/NER/Summary│
          │ + RAG via Vector DB │◄────┐
          └──────────┬──────────┘     │
                     │                │
           ┌─────────▼────────┐       │
           │ Domain Ontology  │       │
           └─────────┬────────┘       │
                     │                │
          ┌──────────▼────────────┐   │
          │ Risk Mapping Module   │   │
          │ (Insurance-specific)  │   │
          └──────────┬────────────┘   │
                     │                │
        ┌────────────▼────────────┐   │
        │ Dashboard / Notifier    │◄──┘
        └─────────────────────────┘


