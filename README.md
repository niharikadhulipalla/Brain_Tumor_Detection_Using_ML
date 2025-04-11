!pip install -q kaggle

from google.colab import files
files.upload()  # Upload kaggle.json here

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

!curl -L -o dataset.zip https://www.kaggle.com/api/v1/datasets/download/josshhh/mri-scans-brain-tumor-image-dataset
! unzip dataset.zip
