# Google Play Store Data in Korea

### Dataset Configuration
1.	PlaystoreData
2.	PlaystoreReviewData
3.	PalystoreBest

#### PlaystoreData
1.	Collection Date : 데이터 수집 날짜 / 형식[2020-06-30 21:30]
2.	App Name : 앱 이름
3.	App Developer : 앱 개발사
4.	App Category : 앱 종류
5.	App Pop Rank : 앱 순위 / numerical
6.	App Download : 앱 설치 수 / numerical
7.  App Review Count : 앱 리뷰 개수
8.	App Charge : 앱 설치 비용 여부 / categorical[Yes : 1 / No : 0]
9.	App Limit : 앱 나이 제한 / numerical

#### PlaystoreReviewData
1.	Collection Date : 데이터 수집 날짜 / 형식[2020-06-30 21:30]
2.	App Name : 앱 이름
3.	Comment Date : 리뷰 날짜
4.	User: 사용자
5.	Rating : 별점 / numerical
6.	Helpful : 유용함 / numerical
7.	Comment : 리뷰 내용
8.	Answer : 개발사 답변

#### PlaystoreBest
1.	Collection Date : 데이터 수집 날짜 / 형식[2020-06-30 21:30]
2.	App Name : 앱 이름
3.	App Developer : 앱 개발사
4.	App Category : 앱 종류
5.	App Best Rank : 앱 순위 / numerical
6.	App Download : 앱 설치 수 / numerical
7.	App Review Count : 앱 리뷰 개수
8.	App Limit : 앱 나이 제한 / numerical

### Data Description
리뷰 수집은 PlaystoreData 및 PlaystoreReviewData를 기준으로 [구글 플레이스토어]-[앱]-[카테고리:게임]-[인기차트]-[인기 앱/게임]에서 수집됩니다.  
각 앱에 대한 리뷰 수집 옵션은 '관련성순, 모든 기기, 평점 전체'의 조건으로 최대 120개까지 수집됩니다.  
Comment는 사용자 리뷰가 공백 포함하여 300자를 넘은 경우에도 전체 리뷰를 모두 반영하여 수집됩니다.  
수집되는 앱의 개수는, 수집되는 매 횟수마다 상위 100개씩 수집됩니다.  
따라서 오류가 발생하지 않았을 경우, 한 수집 당 총 최대 12,000개의 리뷰로 리뷰 내 문장 개수는 제한 없이 수집됩니다.

PlaystoreBest는 [구글 플레이스토어]-[앱]-[카테고리:게임]-[인기차트]-[최고 매출 게임]에서 수집됩니다.
이 데이터셋은 인기 앱/게임에 속하는 게임과 실제 매출을 비교하기 위한 자료입니다.

### Playstore Description
현존하는 마켓의 순위 알고리즘은 정확하게 파악된 바 없습니다.  
구글 측에서는 여러 순위 변동을 통하여 정기적으로 알고리즘이 개선되는 방향으로 발전하고 있음을 알립니다.  
따라서 우리는 다양한 분석가, 마케팅 대행사로부터 다만 추측성 의견을 들을 수 있는 바입니다.  
허나 구글의 플레이스토어의 게임 매출 점유율은 전체 모바일 게임 시장의 약 80%에 육박합니다.  
따라서 이는 소비자들의 의존도가 높아 마켓의 순위 알고리즘의 정밀도와 소비자들의 판단은 별도로 보아야 함을 시사합니다.  
그러므로 이 데이터셋의 순위 기준을 명확하게 알지 못하더라도, 데이터셋을 분석할 가치는 충분하리라 판단합니다.  

### Dataset license
GNU General Public License (GPLv2)
