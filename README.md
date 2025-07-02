# LinkedIn Post Generator Tool (Gen AI Project with Llama 3.2)

This project is an **end-to-end LinkedIn Post Generator** built using **Llama 3.2 (open-source LLM)**, **LangChain**, **Streamlit**, and **Groq Cloud**. It is designed to help LinkedIn influencers and professionals generate high-quality, personalized posts in their unique writing style with just a few clicks.


![Demo of LinkedIn Post Generator](p1.gif)
---

## Features

- **AI-Powered Post Generation:** Leverages Llama 3.2 to generate posts tailored to specific topics and writing styles.
- **Customizable Output:** Users can select topics, post length (short, medium, long), and language (including Hinglish).
- **Topic Extraction:** Automatically analyzes previous posts to extract key topics for future content.
- **Streamlit Frontend:** Intuitive web interface for selecting options and generating posts instantly.
- **Few-Shot Learning:** Uses examples from previous posts to guide the model for more accurate, style-consistent outputs.
- **Cloud Inference:** Integrates with Groq Cloud for fast, scalable model inference—no need to download large models locally.

---

## Technical Architecture

| Stage            | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| Data Collection  | Collects previous LinkedIn posts (manual copy or using datasets).           |
| Preprocessing    | Extracts metadata (topics, language, line count) from posts using LLM.      |
| Enrichment       | Creates enriched JSON with extracted metadata for each post.                |
| Post Generation  | User selects topic, length, and language in Streamlit UI; prompt is created.|
| LLM Inference    | Llama 3.2 generates a new post matching the selected criteria and style.    |

---
