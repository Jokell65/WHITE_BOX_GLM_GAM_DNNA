# GAM-WhiteBoxModel-Analysis
 This repository serves as a resource for implementing and understanding White Box Model and associate Genera Additive Models as a technique as implemented them. Here, you'll find pre-defined models with weights for untrained, trained, and overfitted scenarios. The repository includes my eyenv.zip containing wine quality and other necessary files. The repository also contains some slides explaining the relevance and connection as per the presentation. 
 
# Project structure 

# myenv.zip
Here you can find all the models weights and all other files required to run the gam_1.ipynb code compressed in a zip. Each of the subfolders contains untrained weights, overtrained weights and the best performing weights from the training run. You can also find a simple plot showing the training loss and the validation loss.

**Model Configurations:**
1. **CIFAR-10 Dataset**:
    - **Xavier Uniform Initialization**:
        - [Tanh Activation](model_checkpoints/cifar10/xavier_uniform/tanh/)
        - [ReLU Activation](model_checkpoints/cifar10/xavier_uniform/relu/)
        - [Sigmoid Activation](model_checkpoints/cifar10/xavier_uniform/sigmoid/)
    - **Kaiming Normal Initialization**:
        - [Tanh Activation](model_checkpoints/cifar10/kaiming_normal/tanh/)
        - [ReLU Activation](model_checkpoints/cifar10/kaiming_normal/relu/)
        - [Sigmoid Activation](model_checkpoints/cifar10/kaiming_normal/sigmoid/)
    - **Kaiming Uniform Initialization**:
        - [Tanh Activation](model_checkpoints/cifar10/kaiming_uniform/tanh/)
        - [ReLU Activation](model_checkpoints/cifar10/kaiming_uniform/relu/)
        - [Sigmoid Activation](model_checkpoints/cifar10/kaiming_uniform/sigmoid/)
2. **Wine Quality Dataset**:
    - **Xavier Uniform Initialization**:
        - [Tanh Activation](model_checkpoints/wine_quality/xavier_uniform/tanh/)
        - [ReLU Activation](model_checkpoints/wine_quality/xavier_uniform/relu/)
        - [Sigmoid Activation](model_checkpoints/wine_quality/xavier_uniform/sigmoid/)
    - **Kaiming Normal Initialization**:
        - [Tanh Activation](model_checkpoints/wine_quality/kaiming_normal/tanh/)
        - [ReLU Activation](model_checkpoints/wine_quality/kaiming_normal/relu/)
        - [Sigmoid Activation](model_checkpoints/wine_quality/kaiming_normal/sigmoid/)
    - **Kaiming Uniform Initialization**:
        - [Tanh Activation](model_checkpoints/wine_quality/kaiming_uniform/tanh/)
        - [ReLU Activation](model_checkpoints/wine_quality/kaiming_uniform/relu/)
        - [Sigmoid Activation](model_checkpoints/wine_quality/kaiming_uniform/sigmoid/)


# gam_1.ipynb #

This file can be run to test and train a model features for prediction using a certain configuration.

-To install interpret for GA^2M

```bash
%pip install interpret
```
install dash flask werkzeug
```bash
%pip install --upgrade dash flask werkzeug
```
it may need a specification of version
```bash
%pip install dash==2.0.0 flask==2.0.2 werkzeug==2.0.2
```

## How to Use ##
### Installation ##

**(version of Python == 3.11)**

## 1. Clone the repository: ## 

```bash
   git clone https://github.com/lucasld/neural_network_analysis.git
```

## 2. Navigate to the project directory: ## 

   ```bash
   cd neural_network_analysis
   ```

## 3. Install the required packages (possibly activate/create conda env): ##

 **Run the following command to create a virtual environment** 
    
        ```bash
        python3 -m venv myenv
        ```
**Activate the virtual environment:**
        - **Windows**:
            ```
            myenv\Scripts\activate
            ```
        - **Unix/Linux/macOS**:
            ```
            source myenv/bin/activate
            ```
**Install project dependencies**
```bash
pip install -r requirements.txt
```

## 4. If creating the env from the environment file did not work for you,you can install all dependencies via: ##

**Run one of the 3 commands for cpu, cuda or tpu support respectively:**
```bash
%pip install -U "jax[cpu]"
```
```bash
%pip install -U "jax[cuda12_pip]" -f https://storage.googleapis.com/jax- releases/jax_cuda_releases.html
```
```bash
%pip install -U "jax[tpu]" -f https://storage.googleapis.com/jax-releases/libtpu_releases.html
```
    
**Run the rest:**
```bash
%pip install optax==0.1.7
```
```bash
%pip install scipy==1.11.4
```
    
```bash
%pip install -U "flax[all]"
```
    
```bash
%pip install tensorflow_datasets
```
```bash
%pip install tensorflow
```
```bash
%pip install matplotlib
```
## 5. To run all experiments run: ##
```bash
%sh main.sh
```
**To run a single experiment run:**
```bash
%python main.py cifar10|wine_quality xavier_uniform|glorot_uniform|glorot_normal tanh|relu|sigmoid
```
   


