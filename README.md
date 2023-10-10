# Learning-Install-Text-Generation-Web-UI
Install text generation web ui on windows with nvidia gpu.

1. Install Anaconda
2. Open Anaconda Prompt
3. Enter the following command, do not close Anaconda Prompt

        conda create -n textgen python=3.10.9
        conda activate textgen

4. Install Git, choose your windows version

        https://git-scm.com/download/win

5. Open Git CMD, enter the following command

        git clone https://github.com/oobabooga/text-generation-webui

6. Back to Anaconda Prompt

        cd text-generation-webui
        pip install -r requirements.txt
        conda install torchvision torchaudio pytorch-cuda=11.7 git -c pytorch -c nvidia
        python server.py

If you want to open it directly in the future, in Anaconda Prompt:

        conda activate textgen
        cd text-generation-webui
        python server.py

Open the url.
