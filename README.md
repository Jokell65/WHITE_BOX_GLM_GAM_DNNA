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
git clone https://github.com/Jokell65/WHITE_BOX_GLM_GAM_DNNA.git
```

## 2. Navigate to the project directory: ## 

 ```bash
 cd WHITE_BOX_GLM_GAM_DNNA
 ```
## while there, check out the file listing using. ##

```bash
ls
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

**These maybe apply to mostly GAM, however run dependencies:**
```bash
%pip install numpy
```
```bash
%pip install seaborne
```
```bash
%pip install pandas
```
```bash
%pip onstall matplotlib
```

**These maybe apply to mostly GA^2M, however run dependencies:**
```bash
%pip install interpret
```
```bash
%pip install dash==2.0.0 flask==2.0.2 werkzeug==2.0.2
```
    
```bash
%pip install pandas scikit-learn interpret dash flask werkzeug
```
    
```bash
%pip freeze | grep -E 'dash|flask|werkzeug'
```
```bash
%pip install pandas scikit-learn interpret dash flask werkzeug
```
```bash
%pip install matplotlib
```
## 5. To run all experiments: ##
we suggest that you use juypter notebook and install all dependencies before running gam_1.ipynb
