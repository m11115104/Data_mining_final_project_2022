# 實驗環境

我們使用[Julia](https://julialang.org/)來完成此次的final project並且命名為
>pdMISVM.jl

# 資料集來源

我們使用了[UCI Machine Learning Repository: Musk (Version 1) Data Set](https://archive.ics.uci.edu/ml/datasets/Musk+%28Version+1%29)作為我們執行的dataset

# 執行步驟

0. 下載"Group2_A Linear Primal-Dual Multi-Instance SVM for Big Data Classifications"這個資料夾
1. 開啟Julia console 介面並執行:
   ```
   julia> using Pkg              
   julia> Pkg.activate("path/to/code")          //Data_mining_final_project_2022-main的資料夾路徑
   julia> Pkg.instantiate()
   ```
   
這步驟會為使用者安裝執行時需要的packages，初次執行可能要一段時間

2. 接著，我們對 clean.data 執行 pdMISVM.jl model
   ```
   julia> include("musk_example.jl")
   ```
