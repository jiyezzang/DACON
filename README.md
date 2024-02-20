## 따릉이🚲
서울시 마포구의 날짜별, 시간별 데이터를 바탕으로 따릉이 대여량 예측

## 프로젝트 개요

### 프로젝트 기간

2023.04 ~ 2023.04

### 필요한 라이브러리
``` python

import warnings
warnings.filterwarnings("ignore")

import os
from os.path import join

import pandas as pd
import numpy as np

from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error
from sklearn.ensemble import GradientBoostingRegressor
from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor
from xgboost import XGBRegressor
from lightgbm import LGBMRegressor
import xgboost as xgb
import lightgbm as lgb

from sklearn.model_selection import KFold, cross_val_score

import matplotlib.pyplot as plt
import seaborn as sns

```

## 레퍼런스

matplotlib: 그래프 눈금 간격 지정 방

https://www.dinolabs.ai/88

python을 통한 교차검증(k-fold, stratifiedkFold)

https://continuous-development.tistory.com/166

파이썬 데이터 스케일링(정규화, 표중화) 관련 조언, 방법
https://doong-e.tistory.com/43

Scikit-learn을 이용한 Feature engineering 구현하기
https://techblog-history-younghunjo1.tistory.com/104 
