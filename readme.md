<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project
This project is for the llama2 chatbot built specifically for Mount Holyoke College information. 

### Built With
* ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
* ![JupyterLab](https://img.shields.io/badge/JupyterLab-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
* ![Llama.cpp](https://img.shields.io/badge/Llama.cpp-002b36?style=for-the-badge)
* ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
  
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Prerequisite

### Python library packages
To have all packages to run the code, you can run the below code in the terminal with the main program directory:
```zsh
pip install -r requirements.txt
```
### Architecture
If you are using Apple Silicon (M1) Mac, make sure you have installed a version of Python that supports arm64 architecture; Otherwise, while installing it will build the llama.ccp x86 version which will be 10x slower on Apple Silicon (M1) Mac. To install arm64 architecture on your laptop, run the following code on your laptop:
```zsh
arm64path = "Miniforge3-MacOSX-arm64.sh"
wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh
bash Miniforge3-MacOSX-arm64.sh
```
### Llama.cpp
The main goal of llama.cpp is to run the LLaMA model using 4-bit integer quantization on a MacBook. The instructions below are for Macs with an **M1 chip**.
For other operating systems, comment out those cells and get instructions [here](https://github.com/TrelisResearch/llamacpp-install-basics/blob/main/instructions.md).

```jupyterlab
git clone https://github.com/ggerganov/llama.cpp
%cd llama.cpp
LLAMA_METAL=1 make
%cd ../
```


