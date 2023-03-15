# DataAnalysisTool
  Python pandas, etc.
  - num is numerical, cat is categorical

Python을 이용한 가설 검정 함수
  - 단변량 및 이변량 분석

1. 이변량
  - num 은 숫자형 변수를 의미하며, cat 은 범주형 변수를 의미.

  1) num_num(x, y, data) - 숫자형 변수 - 숫자형 변수 간 이변량 분석
      - scatterplot
      - pearsonr
  2) num_cat(x, y, data) - 숫자형 변수 - 범주형 변수 간 이변량 분석
      - kdeplot
  3) cat_num(x, y, data) - 범주형 변수 - 숫자형 변수 간 이변량 분석
      - barplot
      - category <= 2: t-test, category > 2 : ANOVA
  4) cat_cat(x, y, data) - 범주형 변수 - 범주형 변수 간 이변량 분석
      - mosaic
      - scipy_chi^2 
    
2. 단변량

  1) num_uniV(x, data, bins=20)
    - 숫자형 단변량, x - 변수, data - 데이터, bins - 구간의 갯수 (optional)
  
  2) cat_uniV(x, data)
    - 범주형 단변량 x = 변수, data = 데이터
