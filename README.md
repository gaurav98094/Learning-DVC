### Commands
```
git init
dvc init

mkdir data
# add your data inside data directory

dvc add data/train.csv
git add data/train.csv.dvc data/.gitignore

dvc remote add -d storage gdrive://192Lsv34hDqwIf-lCsVkxgx2CFZstmZTO

pip install dvc-gdrive

git commit -m "Basic Configuration Done"
dvc push


```