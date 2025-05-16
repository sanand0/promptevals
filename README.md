# Prompt Evals

![Prompt Evals Logo](https://img.shields.io/badge/Prompt%20Evals-Optimize%20Your%20Prompts-2563eb)
[![JavaScript](https://img.shields.io/badge/Language-JavaScript-f7df1e)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Bootstrap](https://img.shields.io/badge/Framework-Bootstrap%205-7952b3)](https://getbootstrap.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A [system-prompt learning tool](https://x.com/karpathy/status/1921368644069765486) for evaluating, optimizing, and iterating on AI prompts through a systematic, data-driven approach.

**Links:**

- [Live Demo](https://sanand0.github.io/promptevals)
- [GitHub Repository](https://github.com/sanand0/promptevals)

## Overview

Prompt Evals helps you systematically evaluate and improve AI prompts. By using a data-driven approach, it allows you to:

1. Generate optimized prompts based on input-output examples
2. Test prompts against your dataset
3. Evaluate the quality of generated outputs against expected results
4. Analyze performance using embedding similarity and custom criteria
5. Iteratively refine prompts based on performance data

This is ideal for AI engineers, prompt engineers, and researchers who want to optimize their interactions with large language models.

## Features

- **Prompt Generation**: Automatically generate effective prompts based on example input-output pairs
- **Batch Output Generation**: Test your prompts on multiple inputs in one go
- **Embedding Similarity Analysis**: Measure how closely generated outputs match expected results
- **Custom Evaluation Criteria**: Define and assess specific criteria for what makes a good output
- **Prompt Revision**: Get AI-assisted suggestions to improve underperforming prompts
- **Experiment History**: Track prompt performance across multiple iterations
- **Dark/Light Mode**: Comfortable viewing experience in any environment
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Usage

- **Preparing Your Dataset**. Create a dataset with inputs in the first column and expected outputs in the second column. You can paste data directly or load a CSV file. Example format:
  ```
  Input text<TAB>Expected output text
  Another input<TAB>Another expected output
  ```
- **Generating a Prompt**: Select the number of samples to use. Choose a prompt generation model. Click "Generate prompt"
- **Testing Your Prompt**: Select an output model. Click "Generate output". Review the results in the table
- **Evaluating Performance**: Adjust the embedding similarity threshold. Define your evaluation criteria. Click "Evaluate prompt". Review scores and performance metrics
- **Revising Your Prompt**: Set the number of examples to use. Choose a revision model. Click "Revise prompt". Review and apply the suggested improvements

This process creates a virtuous cycle of continuous improvement for your prompts.

## Demo

The application includes a sample dataset for [clinical trial protocol explanations](clinical-trial-protocol-explanation.csv). This demonstrates how to optimize prompts that explain complex medical protocols in patient-friendly language.

## Installation

### Web Application

No installation required. Access the [live demo](https://sanand0.github.io/promptevals) through any modern web browser.

### Local Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/sanand0/promptevals.git
   cd promptevals
   ```
2. Serve the files using any web server:

   ```bash
   # Using Python's built-in server
   python -m http.server 8000

   # Or using Node.js with http-server
   npx http-server
   ```

3. Open `http://localhost:8000` in your browser
4. Log in with your LLM Foundry credentials

## License

[MIT License](LICENSE)
