## **1. 배경**
*   회사 내에서 업무 성과를 올리고 있는 직원들이 증가하는 추세를 보입니다. 그래서 회사 내에서 우수한 성과를 올리는 직원들이 나오는 요인들을 확인고자 분석하게 되었습니다.

## **2. 데이터**
*  종속변수는 업무성과(PerformanceRating)으로 설정하고, 독립변수들은 업무성과와 관련성이 높아보이는 급여의 증가분 백분율(PercentsalaryHike), 현재 역할의 년수(YearsWithCurrManager), 마지막 프로모션 년수(YearsSinceLastPromotion)을 중심으로 분석하였습니다.

## **3. 분석**
*  일반 통계 분석, 상관관계 분석, 회귀분석 모델을 이용하여 분석하였습니다.

     * 일반 통계 분석
       - 히스토그램을 이용하여 분석한 결과 총 데이터셋 인원 1,470명 중 업무성과에서 3점을 받은 인원수는 1,244명, 4점을 받은 인원은 226명이었습니다.
       - 업무성과와 급여의 증가분 백분율(PercentSalaryHike)의 관계를 비교했을 때, 4점인 경우 평균 21.84%, 3점은 평균 14.0%였습니다.
       - 현재 역할의 년수와 비교했을 때는 3점일 경우 평균 4.18년, 4점일 경우 4.23년으로 크게 차이가 있지 않았습니다. 
         마지막 승진 년수와 비교하였을 때 3점일 경우 평균 2.163년, 4점일 경우 2.323년으로 역시 차이가 많이 나지 않았습니다.
         경력기간(TotalWorkingYears), 일과 생활의 균형정도(WorkLifeBalance), 스톡옵션 정도(StockOptionLevel)은 거의 업무성과가
         동일하여 영향을 미치지 못하는 것으로 보입니다.
  
     * 상관관계 분석
       - 업무성과가 어떤 요인에 의해 영향을 받는지 알기 위해 흔히 사용되는 상관관계를 먼저 사용하였습니다.상관관계를 분석한 결과,
         급여의 증가분 백분율(PercentSalaryHike) 변수가 0.77로 가장 강한 관계를 가지고 있었습니다.
       - 그 외에는 현재 역할의 년수(YearsInCurrentRole) 0.035, 집과의 거리(DistanceFromHome) 0.027,
         현재 관리자와 함께 보낸시간(YearsWithCurrManager) 0.023, 마지막 프로모션(YearsSinceLastPromotion) 0.018로 양의 상관관계를 가졌습니다.
       - 하지만 상관관계 분석을 하였어도 독립변수가 종속변수인 업무성과에 영향을 준다는 인과관계를 결정할 수 없기 때문에 추가적으로 회귀분석을 이용하여 분석하였습니다.
  
     *  회귀 분석
        - 처음 회귀분석을 시행하였을 때 결정계수가 0.6이어서 종속변수를 설명하는데는 조금 강하다고 볼 수 없었습니다.
          그리고 모든 변수의 p값을 보면 집과의 거리, 현재 관리자와 함께 보낸 시간을 제외하고는 0.05 미만으로 나타났습니다
        - 결정계수가 높게 나올 수 있을 것이라 예상하고 p값이 유의하지 않았던 집과의 거리, 현재 관리자와 함께 보낸 시간을 제외한 나머지 변수들을 이용해 회귀분석을 실행하였습니다.
          결정계수의 값은 그래도 0.6이었지만, 모든 변수들의 p값은 유의하게 나타났습니다.
          + 급여의 증가분 백분율이 1% 오르면 업무성과가 0.0763점 상승
          + 현재 역할의 년수가 1년 증가하면 업무성과가 0.0024점 상승
          + 마지막 프로모션 년수가 1년 증가하면 업무성과가 0.0024점 상승

## **4. 결과**
    *   상관관계분석과 회귀분석을 통해 급여의 증가분 백분율이 업무 성과에 영향을 줄 수 있다는 것을 알 수 있었음
    *   추가적으로 일과 생활의 균형정도, 스톡옵션 정도, 경력기간을 포함시켜 위해서 분석했던 마지막 승진, 현재 역할의 년수 등과 같이 회귀분석 실행함. 
        하지만 추가하였던 일과 생활의 균형정도, 스톡욥션 정도, 경력 기간의 p값이 0.5 이상이여서 유의하지 않게 나타남.
    *   따라서 직원들의 업무 성과를 높이는데 결정적인 요인이 된 것은 급여의 증가분 백분율임
        성과금 등을 지불하는 것도 중요하지만 급여의 증가분 백분율을 높이기 위해서는 직원별 성과를 상세히 파악하여 업무 평가 과정에 반영


## **5. 기대효과**
    *  결과를 기반으로 업무평가 내용을 현재의 역할에 대한 평가 등 조금 더 세부적인 항목으로 만들어 성과를 평가한다면 급여의 증가분 백분율을 높임과 동시에 업무성과를
       높일 수 있음
