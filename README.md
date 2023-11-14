<div align="center">

<h1>RVC GUI<br><br>
  
For audio file inference only

  <br>

  

</div>

  

 

  
## GUI

![GUI](https://github.com/Tiger14n/RVC-GUI/raw/main/docs/GUI.JPG)
 <br><br>
  
<br><br>
## Preparing the environment


* Install Python version +3.8 if you have not:
* DONWLOAD https://www.python.org/downloads/

* Execute these commands

MacOS
```
python3 -m pip install -U pip setuptools wheel
pip install -U torch torchaudio 
pip install -r requirements.txt
```

Apple silicon Macs fix
```
pip install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu

export PYTORCH_ENABLE_MPS_FALLBACK=1
```
<br>

* Downlaod [hubert_base.pt](https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/hubert_base.pt/) and place it in the root folder

<br>
 
* Then use this command to start RVC GUI:
```bash
python rvcgui.py
```

# Loading models
use the import button to import a model from a zip file, 
* The .zip must contain the ".pth" weight file. 
* The .zip is recommended to contain the feature retrieval files ".index"

Or place the model manually in root/models
```
models
├───Person1
│   ├───xxxx.pth
│   ├───xxxx.index
│   └───xxxx.npy
└───Person2
    ├───xxxx.pth
    ├───...
    └───...
````
<br>

