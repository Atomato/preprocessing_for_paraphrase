The origin code is from [https://github.com/becxer/cnn-dailymail/](https://github.com/becxer/cnn-dailymail/)

# Instructions
It processes your .xlsx file into the binary format expected by the [code](https://github.com/Atomato/Reinforce-Paraphrase-Generation).

# How to use?
## 1. Process .xlsx file into .story file (train and validation set)
USAGE: python make_stories.py <xlsx_path>
```
python make_stories.py data/paraphrase_data.xlsx
```

## 2. Process .tsv file into .story file (test set)
USAGE: python tsv_to_stories.py <tsv_dir>
```
python tsv_to_stories.py data/tsv_result
```

## 3. Process .story file into .bin
USAGE : python make_datafiles.py
```
python make_datafiles.py
```

## 4. Use the output data
Copy the output data to path/to/Reinforce-Paraphrase-Generation/data/kor/
```
cp ./output/finished_files/vocab path/to/Reinforce-Paraphrase-Generation/data/kor/
cp ./output/finished_files/chunked/train_000.bin path/to/Reinforce-Paraphrase-Generation/data/kor/chunked/train_000.bin
cp ./output/finished_files/chunked/val_000.bin path/to/Reinforce-Paraphrase-Generation/data/kor/chunked/val_000.bin
cp ./output/finished_files/chunked/test_000.bin path/to/Reinforce-Paraphrase-Generation/data/kor/chunked/test_000.bin
```
