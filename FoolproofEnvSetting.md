# Foolproof Python Environment Setting in Win 10
## Using Anaconda/VS Code/TF 2.1
###### This is written for myself to remind me how to set an environment in Win 10.

1. Download and install [Anaconda](https://www.anaconda.com/) and [VS Code](https://code.visualstudio.com/). Make sure they are the newest versions. 
2. Open "Anaconda Prompt" in Start Menu of the OS. Use pip to get newer version of TF. 
    ```
    pip install tensorflow==2.1 
    ```
    If you are in China you may need a VPN. I used to install TF successfully in university but I can't download it at home. Using the mirror version by Tsinghua may report an error, at least it reported bunch of errors for me.
3. Set up your VS Code. Install Python plugin. Then, 
    * python.pythonPath → ...\anaconda3\python.exe
    * python.condaPath → ...\anaconda3\condabin\
    * python.linting.pylintArgs → Add "--generate-members"
4. Test your env. Just like:
    ```
    import tensorflow as tf
    print(tf.__version__)
    ```
    Run it in VS Code, and see if there is something wrong.
