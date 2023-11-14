<div align="center">

<h1>RVC GUI<br><br>
  
*RVC GUI MODIFICADO PARA MACOS INTEL 🇧🇷
em breve para M1/M2/M3
  <br>

  

</div>

  

 

  
## GUI

![GUI](https://github.com/Tiger14n/RVC-GUI/raw/main/docs/GUI.JPG)
 <br><br>
  
<br><br>
## PREPARANDO SUA MAQUINA


* INSTALE O PYTHON VERSÃO +3.8:
* DONWLOAD https://www.python.org/downloads/
  Caso tiver problemas instale outras versões

* EXECUTE ESTES COMANDOS

```
python -m pip install -U pip setuptools wheel
pip install -U torch torchaudio 
pip install -r requirements.txt
```

* SE TIVER PROBLEMAS EXECUTE ESTES
```
python3 -m pip install -U pip setuptools wheel
pip3 install -U torch torchaudio 
pip3 install -r requirements.txt
```

* CORRIJA PROBLEMAS DO APPLE SILICON COM ESTES COMANDOS(M1/M2/M3)
```
pip install --pre torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/nightly/cpu

export PYTORCH_ENABLE_MPS_FALLBACK=1
```
<br>

* BAIXE [hubert_base.pt](https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/hubert_base.pt/) E COLE NA PASTA RAIZ DO PROGRAMA

<br>
 
* USE ESTES COMANDOS PARA INICIAR O RVC GUI NO MACOS:
```bash
cd (ARRASTE A PASTA DO RVC PARA DENTRO DO TERMINAL OU COLE O ENDEREÇO DA LOCALIZAÇÃO DA PASTA)
```
 POR EXEMPLO : ( cd /user/desktop/RVC_GUI/) e em seguida:
```bash
python3 rvcgui.py
```
ou simplesmente abra o terminal e digite: (python3)  de um espaço e arraste o arquivo RVC_gui.py dentro do terminal e de ENTER(RETURN)

# CARREGANDO MODELOS
use o botão importar para importar um modelo de um arquivo zip,
* O .zip deve conter o arquivo de peso ".pth".
* O .zip é recomendado para conter os arquivos de recuperação de recursos ".index"

Ou coloque o modelo manualmente em root/models
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

