# Visually-Grounded-NLG

This project is inspired by the paper "Retrieve, Caption, Generate: Visual Grounding for Enhancing Commonsense in Text Generation Models" by  
Steven Y. Feng, Kevin Lu, Zhuofu Tao, Malihe Alikhani, Teruko Mitamura, Eduard Hovy, Varun Gangal.\n\n

In this project, I used the Common Gen Dataset, which is a benchmark for constrained Natural Language Generation tasks.I performed webscraping to retrieve images corresponding to the concept sets.
The retrieved images were then captioned using 2 image captioning models - BLIP and Vit-GPT2 and the the generated captions were compared basis their coverage. And it was observed that BLIP performed better
on our dataset.The concept sets augmented with these captions were then fed into the T5-base model for finetuning.
The Bleu scores were compared to the model without augmented captions and there was a significant increase in the former.
This proves that visual grounding instills commonsense in text generation models and improves its performance in the NLG task.\n\n

The same has been demonstrated by the code in the Jupyter notebook attached above.
