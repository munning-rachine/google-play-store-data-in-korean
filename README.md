# Google Play Store Data in Korea

### Dataset Configuration
1.	PlaystoreData
2.	PlaystoreReviewData

#### PlaystoreData
1.	Collection Date : 데이터 수집 날짜 / 형식[2020-06-30]
2.	App Name : 앱 이름
3.	App Developer : 앱 개발사
4.	App Category : 앱 종류
5.	App Rank : 앱 순위 / numerical
6.	App Download : 앱 설치 수 / numerical
7.	App Charge : 앱 설치 비용 여부 / categorical[Yes : 1 / No : 0]
8.	App Limit : 앱 나이 제한 / numerical

#### PlaystoreReviewData
1.	App Name : 앱 이름
2.	Comment Date : 리뷰 날짜
3.	User: 사용자
4.	Rating : 별점 / numerical
5.	Helpful : 유용함 / numerical
6.	Comment : 리뷰 내용
7.	Answer : 개발사 답변

### Data Description
리뷰 수집은 무료 앱의 경우 [구글 플레이스토어]-[앱]-[카테고리:게임]-[인기차트]-[인기 앱/게임]에서 수집됩니다.
각 앱에 대한 리뷰 수집 옵션은 관련성순, 모든 기기, 별 1개부터 별 5개까지 각 100개씩 한 앱 당 총 500개씩 수집됩니다. Comment는 사용자 리뷰가 공백 포함하여 300자를 넘은 경우에도 전체 리뷰를 모두 반영하여 수집됩니다. 
수집되는 앱의 개수는, 수집되는 매 횟수마다 상위 10개씩 수집됩니다.
따라서 한 수집 당 총 5000개의 리뷰가 수집되며, 리뷰의 문장 개수는 제한이 없습니다.

### Dataset license
GNU General Public License (GPLv2)
