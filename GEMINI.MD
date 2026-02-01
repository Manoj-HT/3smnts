# Data Creation Context for `bda.json`

This document records the context and methodology used to populate the `bda.json` file with Big Data Analytics notes.

## Project Overview
The goal was to create a JSON file acting as a knowledge base for "Big Data Analytics" topics. The user provided specific topics, and the AI agent generated detailed, structured answers for each.

## Workflow
1.  **User Input:** The user supplied individual topics (e.g., "MongoDB collections", "Spark Architecture", "Kafka").
2.  **Content Generation:** The AI agent generated a comprehensive answer for each topic, suitable for a 7-mark question.
3.  **Formatting & Storage:** The data was appended to `bda.json` adhering to strict formatting constraints.

## Data Format Constraints
The `bda.json` file follows a specific structure:
*   **File Type:** JSON Key-Value pairs.
*   **Key:** The topic name converted to `kebab-case` (e.g., "Spark SQL" -> `spark-sql`).
*   **Value:** A single string containing the detailed answer.
    *   **Length/Detail:** The answer is detailed enough to be worth ~7 marks.
    *   **Line Breaks:** The answer is a single line in the JSON source. Visual line breaks and points are denoted by the `\n` escape character.
    *   **Content:** Answers typically include a definition followed by approximately 7 numbered key points or features.

## Example Entry
```json
"spark-ml": "Spark ML (also known as MLlib) is Apache Spark's scalable machine learning library designed to make practical machine learning scalable and easy.\n1. Unified API – It provides a high-level DataFrame-based API ('spark.ml')...\n2. Comprehensive Algorithms – Includes a wide array of common ML algorithms...\n..."
```

## Session Details
*   **Date:** Sunday, 1 February 2026
*   **User:** manu
*   **System:** Linux
