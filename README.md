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


# Delete everything and then
dvc pull

# Now modify the dataset
dvc diff
dvc add data/train.csv
git commit -m "Modifed Dataset"
dvc push
```

# Moving Back in time
```
git log --oneline
git checkout HEAD^1 data/train.csv.dvc
dvc checkout
```