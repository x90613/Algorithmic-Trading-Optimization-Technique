## About this Project
This project will implement the optimization technique for the "Advanced Group Trading Strategy Portfolio(AGTSP)" based on the original theory. It expands the types and quantities of technical indicators and improves the fitness function. Leveraging genetic algorithm (GA), it learns the information embedded in technical indicators and transforms it into trading strategies suitable for investors' use. The proposed methods will be listed in the user interface along with the obtained trading strategy portfolios, average returns, and maximum risks. Therefore, this project aims to develop an "Advanced Group Trading Strategy Portfolio Trading System."

## Reference 

- [FCC13] T.-C. Fu, C.-P. Chung, and F.-L. Chung, ‘‘Adopting genetic algorithms for technical analysis and portfolio management,’’ Comput. Math. Appl., vol. 66, no. 10, pp. 1743–1757, 2013.
- [CC10] Y.-W. C. Chien and Y. L. Chen, ‘‘Mining associative classification rules with stock trading data—A GA-based method,’’ Knowl.-Based Syst., vol. 23, no. 6, pp. 605–614, 2010.
- [CKC+14] Y.-H. Chou, S.-Y. Kuo, C.-Y. Chen, and H.-C. Chao, ‘‘A rule-based dynamic decision-making stock trading system based on quantum-inspired tabu search algorithm,’’ IEEE Access, vol. 2, pp. 883–896, 2014.
- [CKK14] Y.-H. Chou, S.-Y. Kuo, and C. Kuo, ‘‘A dynamic stock trading system based on a multi-objective quantum-inspired tabu search algorithm,’’ in Proc. IEEE Int. Conf. Syst., Man, Cybern., Oct. 2014, pp. 112–119.
- [CL16] Y.-H. Chang and M.-S. Lee, ‘‘Incorporating Markov decision process on genetic algorithms to formulate trading strategies for stock markets,’’ Appl. Soft Comput., vol. 52, no. 10, pp. 1143–1153, 2016. 
- [LC11] Y. Leu and T.-I. Chiu, ‘‘An effective stock portfolio trading strategy using genetic algorithms and weighted fuzzy time series,’’ in Proc. North-East Asia Symp. Nano, Inf. Technol. Rel., 2011, pp. 70–75. 
- [BLL+16] J. M. Berutich, F. López, F. Luna, and D. Quintana, ‘‘Robust technical trading strategies using GP for algorithmic portfolio selection,’’ Expert Syst. Appl., vol. 46, pp. 307–315, Mar. 2016.
- [CHW+09] J.-S. Chen, J.-L. Hou, S.-M. Wu, and Y.-W. Chang-Chien, ‘‘Constructing investment strategy portfolios by combination genetic algorithms,’’ Expert Syst. Appl., vol. 36, no. 2, pp. 3824–3828, 2009. 
- [CCL+19] Chun-Hao Chen, Yu-Hsuan Chen, Jerry Chun-Wei Lin, and Mu-En Wu, ‘‘An Effective Approach for Obtaining a Group Trading Strategy Portfolio Using Grouping Genetic Algorithm’’ IEEE Access, vol. 7, pp. 7313–7325, 2019. 
- [MF17] M. Kampouridis and F. E. B. Otero, ‘‘Evolving trading strategies using directional changes,’’ Expert Syst. Appl., vol. 73, pp. 145–160, May 2017.
- [WMW+18] D. Wen, C. Ma, G.-J. Wang, and S. Wang, ‘‘Investigating the features of pairs trading strategy: A network perspective on the Chinese stock market,’’ Phys. A, Stat. Mech. Appl., vol. 505, pp. 903–918, Sep. 2018.
- [SN18] S. K. Chandrinos and N. D. Lagaros, ‘‘Construction of currency portfolios by means of an optimized investment strategy,’’ Oper. Res. Perspect., vol. 5, pp. 32–44, 2018.

## Project Tree
```
Algorithmic Trading Optimization Technique
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
│     ├─ 2308.TW (...)
│     │ 
│     ├─ 2330.TW (...)
│     │  
│     ├─ 2344.TW (...)
│     │  
│     ├─ 2412.TW (...)
│     │  
│     ├─ 2413.TW (...)
│     │ 
│     ├─ 2603.TW (...)
│     │  
│     └─ META (...)
│      
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
