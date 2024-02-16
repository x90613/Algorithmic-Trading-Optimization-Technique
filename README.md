# About this Project

This project will implement the optimization technique for the "Advanced Group Trading Strategy Portfolio(AGTSP)" based on the original theory [1]. It expands the types and quantities of technical indicators and improves the fitness function. Leveraging genetic algorithm (GA), it learns the information embedded in technical indicators and transforms it into trading strategies suitable for investors' use. The proposed methods will be listed in the user interface along with the obtained trading strategy portfolios, average returns, and maximum risks. Therefore, this project aims to develop an "Advanced Group Trading Strategy Portfolio Trading System."

[1] [An Effective Approach for Obtaining a Group Trading Strategy Portfolio Using Grouping Genetic Algorithm](https://ieeexplore.ieee.org/abstract/document/8604011)

## Run the project

Please wait...

## Project Tree
```
AGTSP
├─  Experimental data
│  ├─ 0050 top15 .zip
│  ├─ 九份 0050 Top555.zip
│  └─ 九份 META Top555.zip
├─ .gitignore
├─ README.md
├─ data
│  └─ stock
│     ├─ 0050.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  ├─ Top15.json
│     │  │  ├─ Top555.json
│     │  │  └─ Top777.json
│     │  ├─ ValidationData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  └─ TIvalue.json
│     │  └─ block.json
│     ├─ 2308.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  └─ Top555.json
│     │  ├─ ValidationData
│     │  │  ├─ Date.json
│     │  │  └─ StockData.json
│     │  └─ block.json
│     ├─ 2330.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  ├─ TIvalue2.json
│     │  │  ├─ Table.json
│     │  │  ├─ Top15.json
│     │  │  ├─ Top21_Debug.json
│     │  │  └─ Top555.json
│     │  ├─ ValidationData
│     │  │  ├─ Date.json
│     │  │  └─ StockData.json
│     │  └─ block.json
│     ├─ 2344.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  └─ Top555.json
│     │  └─ ValidationData
│     │     ├─ Date.json
│     │     └─ StockData.json
│     ├─ 2412.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  └─ Top555.json
│     │  └─ ValidationData
│     │     ├─ Date.json
│     │     ├─ Signal.json
│     │     ├─ StockData.json
│     │     └─ TIvalue.json
│     ├─ 2413.TW
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  └─ Top555.json
│     │  ├─ ValidationData
│     │  │  ├─ Date.json
│     │  │  └─ StockData.json
│     │  └─ block.json
│     ├─ 2603.TW
│     │  ├─ History
│     │  ├─ TrainingData
│     │  │  ├─ Date.json
│     │  │  ├─ Signal - 複製.json
│     │  │  ├─ Signal.json
│     │  │  ├─ StockData.json
│     │  │  ├─ TIvalue.json
│     │  │  ├─ Table - 複製.json
│     │  │  ├─ Table2.json
│     │  │  └─ Top555.json
│     │  ├─ ValidationData
│     │  │  ├─ Date.json
│     │  │  └─ StockData.json
│     │  └─ block.json
│     └─ META
│        ├─ TrainingData
│        │  ├─ Date.json
│        │  ├─ Signal.json
│        │  ├─ StockData.json
│        │  ├─ TIvalue.json
│        │  └─ Top555.json
│        ├─ ValidationData
│        │  ├─ Date.json
│        │  ├─ Signal.json
│        │  ├─ StockData.json
│        │  └─ TIvalue.json
│        └─ block.json
└─ main
   ├─ Algo
   │  ├─ BackTesting.py
   │  ├─ Chromosome.py
   │  ├─ Population.py
   │  ├─ __init__.py
   │  └─ __pycache__
   │     ├─ Chromosome.cpython-39.pyc
   │     ├─ Population.cpython-39.pyc
   │     └─ __init__.cpython-39.pyc
   ├─ PreProCessing
   │  ├─ CalculateTIvalue.py
   │  ├─ Case
   │  │  ├─ Case.py
   │  │  ├─ TIformat.json
   │  │  ├─ __pycache__
   │  │  │  └─ Case.cpython-39.pyc
   │  │  ├─ oldCase .py
   │  │  └─ oldTIformat.json
   │  ├─ DownloadData.py
   │  ├─ TI2Ranking.py
   │  ├─ TI2Signal.py
   │  ├─ __init__.py
   │  ├─ __pycache__
   │  │  ├─ CalculateTIvalue.cpython-39.pyc
   │  │  ├─ Case.cpython-39.pyc
   │  │  ├─ Cov2Image.cpython-39.pyc
   │  │  ├─ DownloadData.cpython-38.pyc
   │  │  ├─ DownloadData.cpython-39.pyc
   │  │  ├─ Ranking.cpython-39.pyc
   │  │  ├─ SettingFile.cpython-39.pyc
   │  │  ├─ TI2Ranking.cpython-39.pyc
   │  │  ├─ TI2Signal.cpython-39.pyc
   │  │  ├─ __init__.cpython-38.pyc
   │  │  └─ __init__.cpython-39.pyc
   │  ├─ dask-worker-space
   │  │  ├─ global.lock
   │  │  └─ purge.lock
   │  └─ oldfunctions
   │     ├─ OldDask_TI2Ranking.py
   │     ├─ OldRanking.py
   │     ├─ ProductFiles.py
   │     └─ Ranking.py
   ├─ RFiles.py
   ├─ SettingFile.py
   ├─ SignalMap.json
   ├─ TI_List.json
   ├─ __pycache__
   │  ├─ RFiles.cpython-39.pyc
   │  └─ SettingFile.cpython-39.pyc
   ├─ dask-worker-space
   │  ├─ global.lock
   │  └─ purge.lock
   ├─ main.py
   └─ setting.json

```
