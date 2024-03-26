## Localhost

Install [Python 3.10.6](https://www.python.org/downloads/release/python-3106/).

```sh
where python
...\python -m venv venv
venv\Scripts\activate.bat
```

Edit `requirements.txt`:

```
torchvision==0.15.2
# torch
```

```sh
pip install -r requirements.txt
pip install git+https://github.com/kodalli/pydensecrf.git
```

Install [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit), I use `CUDA 11.8`. Check it:

```sh
echo %CUDA_PATH%
echo %CUDA_PATH_V11_8%
```

Downloads `torch-2.0.1+cu118-cp310-cp310-win_amd64` from https://download.pytorch.org/whl/torch.

```sh
pip install ...\torch-2.0.1+cu118-cp310-cp310-win_amd64
```

```sh
python -m manga_translator -v --mode web --use-gpu
```

## Troubleshoot

- [Upgrading PyTorch to v2.0.1 and torchvision to v0.15.2 and torchaudio to v2.0.2](https://github.com/googlecolab/colabtools/issues/3646)