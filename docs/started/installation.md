LEGENT currently support Windows/Linux/MacOS.
Support for WebGL will be available soon.

## Install LEGENT:
``` bash
git clone https://github.com/chengzl18/LEGENT.git
cd LEGENT
pip install -e .
```

## Download Game Client
Download from [Hugging Face](https://huggingface.co/chengzl18/legent-client/tree/main) and extract the file.
For Linux user, you need to modify file permissions.

For example:
```
wget https://huggingface.co/chengzl18/legent-client/resolve/main/legent-linux-server.zip
unzip legent-linux-server.zip
chmod -R 777 legent-linux-server/*
```

## Run On Linux Server
For a Linux server without a graphical interface, you need to install Xvfb to support game rendering.

if you have root access to the server, you can install Xvfb by using:
```
sudo apt install xvfb
```

Prepend `xvfb-run` to commands running Python scripts. For example:
```
xvfb-run python demo.py
```