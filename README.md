# AI SQL Engineer

This project implements an AI SQL engineer capable of performing SQL queries on a .csv file. The AI SQL engineer utilizes a fine-tuned language model (LLM) to interpret natural language questions and generate SQL queries.

## Features

- **Natural Language Interface**: Users can ask questions in natural language.
- **CSV Input**: The AI SQL engineer accepts a .csv file as input.
- **SQL Query Generation**: The AI SQL engineer generates SQL queries based on the input question.
- **Backend Options**: The AI SQL engineer can use Mistral, Gemma, or the Groq API in the backend.

## Setup

1. Clone the repository:

   ```sh
   git clone https://github.com/<your-username>/ai-sql-engineer.git

2. Install dependencies:

    ```sh
     pip  install -r requirements.txt

3.Fine-tuned LLMs:

Mistral and Gemma Link :- https://huggingface.co/gaurav16/SQL-Models/tree/main

## Usage

1. Ensure your .csv file is formatted correctly.
2. Run the AI SQL engineer:

   ```sh
   python main.py
Input your natural language question. For example:

csharp
What is the total sales by region?
View the generated SQL query and output. For the example question above, the output might be:

sql
Copy code
SELECT region, SUM(sales) AS total_sales FROM table GROUP BY region;
diff
Copy code
+------------+-------------+
|   region   | total_sales |
+------------+-------------+
|  Region1   |   10000     |
|  Region2   |   15000     |
|  Region3   |   12000     |
+------------+-------------+
The AI SQL engineer will execute the SQL query on the .csv file and display the results.
