# 📊 Fine-tune LLaMA3 for Item Price Prediction:

This project aims to predict **Amazon item prices** using a combination of traditional machine learning models and large language models (LLMs). The objective is to compare the performance of these models and evaluate how **fine-tuning LLMs** like **GPT-4o-mini** and **LLaMA3.1** can improve prediction accuracy.

Additionally, the fine-tuning process is tracked and monitored using Weights & Biases.

## 📚 Dataset

We used the McAuley-Lab/Amazon-Reviews-2023 dataset, available on Hugging Face.

### 🛠️ Models Used

This project utilizes both **traditional machine learning** models and **LLMs**:

Machine Learning Models

	•	Linear Regression
	•	Bag of Words
	•	Word2Vec
	•	Random Forest

Large Language Models (LLMs)

	•	GPT-4o-mini
	•	LLaMA3.1

## 🧰 Tools and Libraries

	•	Jupyter Notebook: For experimentation and model development.
  •	GoogleColab for GPU finetuning.
  •	Weights & Biases (W&B): For monitoring the fine-tuning process and tracking model performance.w32
  •	Huggingface.
  •	**QLoRA** & **Peft** for LLM finetuning.
  

## 🚀 Results

### Performance Summary

	•	Among the machine learning models, Random Forest + Linear Regression achieved the best performance.
	•	GPT-4o-mini outperformed all other models (including ML models) when used without fine-tuning.

### Fine-Tuning LLMs

	•	GPT-4o-mini fine-tuning:
	  •	Interestingly, the performance of GPT-4o-mini slightly worsened after fine-tuning.
	•	Possible reasons:
	  •	Overfitting to the fine-tuning dataset.
	  •	Loss of generalization due to the fine-tuning process altering the model’s prior knowledge.
	• LLaMA3.1 fine-tuning:
	  •	After fine-tuning, LLaMA3.1 performed better than GPT-4o-mini, showing improved ability to make accurate predictions.
