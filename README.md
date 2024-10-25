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

• Jupyter Notebook: For experimentation and model development.
• GoogleColab for GPU finetuning.
• Weights & Biases (W&B): For monitoring the fine-tuning process and tracking model performance.w32
• Huggingface.
• **QLoRA** & **Peft** for LLM finetuning.
  

## 🚀 Results

### Performance Summary

- Among the machine learning models, Random Forest + Linear Regression achieved the best performance.
	- ![image](https://github.com/user-attachments/assets/5d2fe5f8-a543-4f75-bedf-8fec08907fd2)
 	- ![image](https://github.com/user-attachments/assets/6584bcba-8d90-4ad9-9f3e-4db772400e23)

- GPT-4o-mini outperformed all other models (including ML models) when used without fine-tuning.
	- ![image](https://github.com/user-attachments/assets/c3ec633f-6909-441b-a1bd-663b377a526b)


### Fine-Tuning LLMs

- GPT-4o-mini fine-tuning:
	- Interestingly, the performance of GPT-4o-mini slightly worsened after fine-tuning.
 	-  ![image](https://github.com/user-attachments/assets/14e226bc-046b-4573-85fc-fbf7a4366b9d)
  	-  Possible reasons:
  	-  Overfitting to the fine-tuning dataset.
  	-  Loss of generalization due to the fine-tuning process altering the model’s prior knowledge.
-  LLaMA3.1 fine-tuning:
	- After fine-tuning, LLaMA3.1 performed better than GPT-4o-mini, showing improved ability to make accurate predictions.
 	- ![image](https://github.com/user-attachments/assets/0e1bcb4a-b370-40f3-9f81-d75d64fb304a)

