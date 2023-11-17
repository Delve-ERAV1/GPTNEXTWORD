# S22

# GPT Language Model - Gradio Interface

## Introduction
This repository hosts the Gradio interface for a custom-trained GPT model. It allows users to interact with the model by providing a text prompt and control parameters to generate responses.

## Model Training Details

### Data Configuration
The model was trained on a diverse dataset with the following proportions from the overall corpus:
- arXiv: 5%
- Books: 20%
- Common Crawl (C4): 15%
- Creative Commons (CC): 55%
- Wikipedia: 5%

### Training Parameters
- Learning Rate: 6.00E-03
- Batch Size: 32
- Micro Batch Size: 4 (Gradient Accumulation)
- Max Iterations: 15000
- Weight Decay: 1e-1
- Optimizer Betas: β1 = 0.9, β2 = 0.95
- Gradient Clipping: 1.0
- Learning Rate Decay: Enabled
- Warmup Iterations: 2000
- Learning Rate Decay Iterations: 15000
- Minimum Learning Rate: 6E-6

### Training Log Excerpt
Here's an excerpt from the training log showing the final iterations:


```
iter 10000 step 2500: loss 3.2343, LR: 0.001940, iter time: 114.49ms
iter 10100 step 2525: loss 3.8201, LR: 0.001873, iter time: 117.37ms
... [additional lines omitted for brevity] ...
iter 10900 step 2725: loss 3.4297, LR: 0.001361, iter time: 116.42ms
```

## Usage
Launch the app by running:

```python
gradio app.py
```

Deployed to Huggingface Spaces - 
https://huggingface.co/spaces/Sijuade/GPTNEXTWORD

## Contributing
Contributions are welcome! Please fork the repository and submit pull requests with your proposed changes.

## License
This project is open-sourced under the MIT License.


## Acknowledgments
Gradio for the interactive app framework.
https://github.com/Lightning-AI/lit-gpt
