## Bet! (Team B)
#### 참여자 : 남승우, 김영호, 신재우, 임창
#### EDA 프로젝트 자료 소개
> * Dataset
>   * 연세대학교 상경경영대 전공기본, 전공필수 & 전공선택 강의 일부
>   * https://underwood1.yonsei.ac.kr/com/lgin/SsoCtr/initExtPageWork.do?link=handbList&locale=ko # 데이터 수집 링크
> * [EDA 발표자료](EDA_B조_발표자료.pdf) : EDA 발표 때 사용한 ppt입니다.
> * [EDA 최종 코드](EDA_B조_코드.ipynb) : EDA 발표와 관련하여 사용된 코드입니다.

<br>



## EDA 프로젝트 요약

1. 프로젝트 주제 및 목적
        - Main : 학과별 수강신청 난이도 차이 유무
        - Sub-A : 수강형태 변화에 따른 난이도 차이 유무
        - Sub-B : 강의 평가 지표에 따른 난이도 차이 유무 

3. 데이터 전처리
        - 경로 : [Team_B/Preprocessing.ipynb](https://github.com/namu-tree/10th-EDA/blob/main/Team_B/Preprocessing.ipynb)
        - Column index 제거, txt 확장자명 csv 확장자명으로 변환
        - str type으로 되어있는 범주들 Int type으로 변환
            
 
5. 분석 방법 및 결과
   
   - Main : Kruskal Wallis Test 사용
     - 전공자 : 경제 - 응통과 경영 간 수강신청 성공 비율, 수강신청 실패 최대 마일리지 사이 유의한 차이 존재 
     - 부전공자 : 경제 - 응통과 경영 간 수강신청 성공 비율에 유의한 차이 발생
     - 비전공자 : 세 학과의 수강신청 성공 비율에 유의한 차이 없음 - 수강신청 실패 최대 마일리지도 마찬가지
   - Sub - A : Kruskal Wallis Test 사용
     - 강의 방식에 따라 마일리지 수강신청 난이도의 분포에 차이가 있다고 보기 어려움
   - Sub - B : ANOVA TEST 사용
     - 시험 횟수를 제외하고 모든 요소가 수강 신청 난이도에 유의미하다고 볼 수 있음
		    
7. 결론
  - Main : 전체적으로 경영이 수강신청 난이도가 가장 높고, 경제, 응통 순으로 난이도 분포 확인
  - Sub - A : 강의방식에 따라 마일리지 난이도 분포가 차이 X
  - Sub - B : 시험횟수를 제외한 모든 강의평 요소가 수강신청 난이도에 영향
    
8. 아쉬운 점
    - 학기별 강의 수의 변동성
    - 특정 범주 강의만 데이터셋으로 활용
    - Human Crawling
    - 강의가 개설되는 시간대 고려 X



<br>



 ## 각 팀원의 역할
 
|이름|활동 내용| 
|:---:|:---|
|남승우| - (팀장) 전체 일정 관리 및 회의 진행..<br> - 발표자료 제작 도움| 
|임창재| - 시각화<br> - Main Task 분석 진행 <br> - 발표| 
|김영호| - 시각화 <br> - Sub - A Task 분석 진행 <br> - 발표|
|신재우| - 시각화<br> - Sub - B Task 분석 진행 <br> - 발표| 
<br/>



## tree (가능하다면, github에서 tree 명령어를 통해 전체 파일 트리를 보여주세요)
```bash
├── Dataset
│   ├── dataset1.csv
│   └── dataset2.csv
│
├── 팀장
│   └── dummy.txt
├── 임창재
│   ├── Preprocessing_ChangjaeIm.ipynb
|   └── Lecture_type_preprocessing.ipynb
├── 김영호
│   ├── Preprocessing.ipynb
|   ├── Preprocessing_KimYeongho.ipynb
|   ├── difficulty.ipynb
|   ├── finaldata.csv
|   ├── plot.ipynb
|   └── test.ipynb
├── 신재우
│   └── Preprocessing.ipynb
├── EDA_B조_발표자료.pdf
│   
│
└── README.md
``` 
