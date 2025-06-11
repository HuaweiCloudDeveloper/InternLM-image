# internlm下载指南

## ‌一、环境准备
### 系统配置
> -  服务器：鲲鹏服务器
> -  操作系统：Huawei Cloud EulerOS 2.0 64bit
> - CPU: 4vCPUs 或更高
> - RAM: 16GB 或更大
> - Disk: 至少 40GB
### 更新系统

```bash
sudo yum update -y  
```

### 安装conda创建python环境
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-aarch64.sh

bash Miniconda3-latest-Linux-aarch64.sh

#若安装后无法识别 conda 命令，手动添加路径：
echo 'export PATH="~/miniconda3/bin:$PATH"' >> ~/.bashrc    
source ~/.bashrc  

#创建环境
conda create -n internlm python=3.10
conda activate internlm
```

### 更新pip

```bash
python -m pip install --upgrade pip
```

### 安装torch
```bash
pip install torch==2.2.0 -i https://pypi.tuna.tsinghua.edu.cn/simple
#安装numpy要2以下
pip install "numpy<2"  #numpy==1.26.4
pip install packaging streamlit einops sentencepiece -i https://pypi.tuna.tsinghua.edu.cn/simple
#conda install -c conda-forge transformers==4.4.0
pip install transformers==4.40.2 -i https://pypi.tuna.tsinghua.edu.cn/simple
```
## ‌二、下载模型

### 安装ModelScope
```bash
pip install modelscope -i https://pypi.tuna.tsinghua.edu.cn/simple 
```

### 下载internlm2_5-1_8b-chat模型到当前文件夹
```bash
modelscope download --model Shanghai_AI_Laboratory/internlm2_5-1_8b-chat --local_dir ./dir
```
## ‌三、模型使用
下载代码
InternLMt的github地址：https://github.com/InternLM/InternLM

下载项目代码文件，推理代码在chat/web_demo.py下

需要将模型修改为本地模型地址

代码修改适配，详情见代码仓库:https://gitcode.com/2401_82798006/InternLM/overview