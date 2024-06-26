# Data Mining
- Pandas에 대해서 학습하고 아래의 문제를 해결하기
- <b>하나의 .ipynb파일(쥬피터 랩 확장자)로 답안 파일을 만들고, 각 문제를 블록 단위로 구별하여 코딩할 것.</b>
- <b>코드에 대한 주석 작성 필수</b>
- class 사용 금지
- .xlsx파일을 불러오기 위해선 xlrd와 openpyxl 패키지가 필요함 -> pip 사용!
- 깊은 복사(copy())에러 시 pandas.options.mode.chained_assignment=None 삽입

### 데이터프레임
1. <b>corona.xlsx 파일엔 1월20일 부터 1월30일까지의 중국과 타국에서의 COVID19 확진자 추이가 담겨있다.</b>
    - 이 엑셀을 pandas.DataFrame으로 불러온 뒤 '한국' column을 만들어서 다음의 데이터를 추가하고 covid19.csv로 저장하기
      ```
               한국
      1뭘 20일 : 1
      1월 22일 : 1
      1월 24일 : 2
      1월 26일 : 3
      1월 28일 : 4
      1월 30일 : 7
      ```
    - covid19.csv를 불러와서 원본 데이터는 sheet1에, 중국 데이터는 sheet2에, 타국 데이터는 sheet3에, 한국 데이터는 sheet4에 저장하고 covid19_new.xlsx로 저장하기
</br>
  
2. <b>auto-mpg.csv 파일은 자동차의 연비에 대한 데이터 파일이다.</b>
    - 다음에 맞추어서 해당 데이터셋에 columns name을 설정하고, auto-mpg-2.csv로 저장하기
    ```
    mpg(연비)
    cylinders(실린더수)
    displacement(배기량)
    horsepower(출력)
    weight(차중)
    acceleration(가속능력)
    modelYear(출시년도)
    originNumber(제조국번호)
    name(모델명)
    ```
    - 80년대에 생산된 모델의 모델명만을 출력하라
    - mpg(연비)와 horsepower(출력) 열의 표준편차값을 구하라
    - horsepower(출력) 열의 표준편차는 구할 수 없다. 이유를 서술하라.
    - modelYear(출시년도)를 최신순에 따라 데이터를 정렬해서 auto-mpg-3.csv로 저장하라
</br>

3. <b>남북한발전전력량.xlsx 파일엔 남한과 북한의 발전전력별 연간통계량이 저장되어있다.</b>
    - 해당 데이터를 읽어와서 남한과 북한의 수력 및 화력발전과 그 합계에 대한 연간 통계량만을 분리해서 남북한수력및화력발전전력량.csv로 저장하라. 
</br>

4. <b>다음을 만족하는 20년 달력 데이터 프레임을 만드시오.</b>
    ```
        original    Year    Month    Day    weekday    weekend    season    
    0   20-01-01     20       1       1       Wed         0       winter
    1   20-01-02     20       1       2       Thr         0       winter
    2   20-01-03     20       1       3       Fri         0       winter
    3   20-01-03     20       1       4       Sat         1       winter
    
    ...   ...        ...     ...     ...      ...        ...        ...   
    
    365 20-12-31     20       12      31      Thr         0       winter
    
    ```
