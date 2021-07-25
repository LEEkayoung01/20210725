# 20210725

#1


#2
import numpy as np

revenue_in_yen = [
    300000, 340000, 320000, 360000, 
    440000, 140000, 180000, 340000, 
    330000, 290000, 280000, 380000, 
    170000, 140000, 230000, 390000, 
    400000, 350000, 380000, 150000, 
    110000, 240000, 380000, 380000, 
    340000, 420000, 150000, 130000, 
    360000, 320000, 250000
]

revenue_in_dollar = [
    1200, 1600, 1400, 1300, 
    2100, 1400, 1500, 2100, 
    1500, 1500, 2300, 2100, 
    2800, 2600, 1700, 1400, 
    2100, 2300, 1600, 1800, 
    2200, 2400, 2100, 2800, 
    1900, 2100, 1800, 2200, 
    2100, 1600, 1800
]

#코드를 입력하세요. 
array1 = np.array(revenue_in_yen) * 10.08
array2 = np.array(revenue_in_dollar) * 1138
won_array = array1 + array2
#정답 출력
won_array

1. numpy 연산
    1) 기본연산
        array1 = np.array(리스트) +, -, *, / 연산
        array1 = np.array([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31])
   2) 불린 연산
        array1 > 4   // array([False, False, True, True (...다 나옴) ])
       
        booleans = np.array([False, True])
        np.where(booleans) // (array([1]) // True 인 index 
        
        // array1에 있는 값 중 4보다 큰 것만으로 array를 만들기
        filter = np.where(array1 > 4) // (array1([ 2, 3, 4, 5, 6, 7, 8, 9, 10]) <= 인덱스
        array1[filter] // array([ 5, 7, 11, 13, 17, 23, 30])
                          
  
 #3 흥부부대찌개 목표 일 매출
 import numpy as np

revenue_in_yen = [
    300000, 340000, 320000, 360000, 
    440000, 140000, 180000, 340000, 
    330000, 290000, 280000, 380000, 
    170000, 140000, 230000, 390000, 
    400000, 350000, 380000, 150000, 
    110000, 240000, 380000, 380000, 
    340000, 420000, 150000, 130000, 
    360000, 320000, 250000
]

#코드를 작성하세요.
array1 = np.array(revenue_in_yen)
filter = np.where(array1 < 200000)
bad_days_revenue = array1[filter]
#정답 출력
bad_days_revenue


2. numpy array와 phthon list의 차이점
  1) 문법 차이
    - 덧셈: 
          numpy - 각 인덱스 별로 더함.
          list - 이어붙임.
    - 뺄셈, 곱셈, 나눗셈: 
          numpy: 잘 동작
          list - 오류.
    -  



 

