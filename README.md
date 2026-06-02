# Support Ticket Auto Tagging using LLM (Advanced Version)

## Project Overview
This project is an AI-powered support ticket classification system that automatically assigns relevant tags to customer queries using a transformer-based zero-shot learning model. It also includes a few-shot learning comparison to improve classification performance.

The system predicts the top 3 most relevant categories for each support ticket and provides insights through visualization and dataset analysis.

---

## Dataset Source

The dataset used in this project was obtained from a compressed ZIP file containing a real-world customer support ticket dataset.

- Dataset File: `customer_support_tickets.csv`
- Source: Kaggle (Customer Support Ticket Dataset)
- Format: ZIP file containing CSV
- Extraction: The dataset was uploaded and extracted directly in Google Colab using Python's `zipfile` module

---

## Key Features

- Zero-shot classification using pretrained BART model
- Few-shot learning comparison for improved performance
- Top-3 tag prediction for each support ticket
- Automatic dataset loading from ZIP file
- Visualization of ticket category distribution
- CSV export of final tagged results

---

## Methodology

### 1. Data Loading
- ZIP file uploaded manually in Google Colab
- Extracted using Python `zipfile` module
- CSV file loaded using Pandas

### 2. Preprocessing
- Extracted text column from dataset
- Cleaned missing values
- Converted data into list format for processing

### 3. Model Used
- Facebook BART Large MNLI (`facebook/bart-large-mnli`)
- Used for zero-shot text classification

### 4. Classification Approach
- Input ticket text is compared against predefined labels
- Model returns probability scores for each label
- Top 3 labels selected as predictions

### 5. Few-Shot Enhancement
- Prompt-based classification used for improved accuracy comparison
- Demonstrates difference between zero-shot and guided classification

---

## Labels Used

- Network Issue
- Login Issue
- Billing Issue
- Technical Bug
- Account Issue
- Subscription Issue
- General Inquiry

---

## Results

- Successfully classified support tickets into multiple categories
- Generated top-3 predicted tags for each ticket
- Compared zero-shot vs few-shot performance
- Visualized category distribution using bar charts

---

## Technologies Used

- Python
- Pandas
- Transformers (Hugging Face)
- PyTorch
- Matplotlib
- Scikit-learn

---

## Skills Demonstrated

- Natural Language Processing (NLP)
- Zero-shot learning
- Few-shot learning
- Prompt engineering
- Transformer-based classification
- Data preprocessing and visualization
- Real-world AI automation

---

## Output

The final output includes:
- A CSV file containing tickets with predicted tags
- Visualization of ticket category distribution
- Comparison between zero-shot and few-shot results

---

## File Generated

- `auto_tagged_tickets.csv`

---

## Author

Developed as part of AI/ML Engineering Internship Tasks.

---

## Note

This project demonstrates a real-world AI workflow using pretrained language models without requiring manual training, making it efficient and scalable for production-level support systems.
