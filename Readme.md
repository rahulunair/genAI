# Gen AI Playground on Intel® Data Center GPU Max 1100

Welcome to the Gen AI Playground, a collection of notebooks designed to showcase generative AI workloads on Intel® Data Center GPU Max 1100. These notebooks are designed to be accessible to a broad audience, including AI creators, artists, engineers, and those who are just curious about generative AI.

![Intel Data Center GPU Max 1100](https://intelcorp.scene7.com/is/image/intelcorp/data-center-gpu-max-badge?$64.64$&fmt=png-alpha)

## Table of Contents

- [Welcome Notebook](./welcome.ipynb)
- [Text-to-Image with Stable Diffusion](./text_to_image.ipynb)
- [Image-to-Image with Stable Diffusion](./image_to_image.ipynb)
- [Simple LLM Inference: Playing with Language Models](./simple_llm_inference.ipynb)
- [Code generation using LLMs](./optimize_code_generation_with_llms.ipynb)
- [Gemma model finetuning with SFT and LoRA](./gemma_xpu_finetuning.ipynb)
- [QLoRA finetuning on Intel GPUs](./qlora_finetuning.py)
- Please create an issue here if you want me to add new models and implementations.

## Requirements

### Hardware
- Intel® Data Center GPU Max 1100

### Software
- Python
- PyTorch with Intel Extension for PyTorch
- Jupyter Notebook or Jupyter Lab

## Installation

Run the following commands to set up the necessary software requirements:

```bash
python -m pip install torch==2.0.1a0 torchvision==0.15.2a0 intel_extension_for_pytorch==2.0.110+xpu -f https://developer.intel.com/ipex-whl-stable-xpu
```
For Jupyter Notebook or Jupyter Lab:

```bash
pip install jupyterlab
```

or

```bash
pip install notebook
```

Each notebook contains a first cell that installs additional packages using conda, which assumes you're running inside a conda environment. Here's a sample installation from one of the notebooks:

```bash
import sys
!{sys.executable} -m pip install  invisible-watermark
!conda install -y --quiet -c conda-forge \
    accelerate==0.23.0 \
    validators==0.22.0 \
    diffusers==0.18.2 \
    transformers==4.32.1 \
    tensorboardX \
    pillow \
    ipywidgets \
    ipython \
    sentencepiece
```

## Usage

Simply navigate to one of the notebooks to get started! Each notebook comes with comprehensive guides and examples to help you explore the fascinating world of generative AI.

## License

Apache License.See [LICENSE](./LICENSE) for more details.
