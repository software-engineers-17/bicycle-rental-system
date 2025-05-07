# bicycle-rental-system

공유 자전거 대여 시스템

# 팀 코드

17856

# 역할 분담

분담한 기능에 대하여 requirement list, use case diagram, use case description 를 작성하였습니다.

신형섭 : <br>

- 회원 가입 기능
- 회원 탈퇴 기능
- 로그인/로그아웃 기능

김지우 :<br>

- 대여소 등록/조회/삭제 기능
- 자전거 등록/조회/삭제 기능
- 대여소 검색 기능

임가현 : <br>

- 상세정보 조회 및 자전거 즉시대여/예약대기 기능
- 자전거 대여 정보 조회
- 자전거 예약대기 정보 조회/취소
- 자전거 반납 및 식당 예약 서비스 연계 기능

이예은 : <br>

- 결제 및 요금 조회 기능
- 이용 내역 조회/삭제 기능
- 통계 기능

## Requirement List

| No. | Requirement                                                                                                                                                                                                                                                                   | Use Case                              |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| 1   | System users can register for membership. The required information for membership registration includes ID, password, phone number, payment method, and preferred bike type (standard/electric). The administrator can log in with the given ID (admin) and password (admin). | Regist Membership                     |
| 2   | Members can withdraw their membership at any time. Upon withdrawal, all user privileges and data are deleted.                                                                                                                                                                 | Withdrawal Membership                 |
| 3   | Administrators and members can log in to the system using their ID and password. Upon logout, the system connection is terminated.                                                                                                                                            | Login/ Logout                         |
| 4   |                                                                                                                                                                                                                                                                               |                                       |
| 5   |                                                                                                                                                                                                                                                                               |                                       |
| 6   |                                                                                                                                                                                                                                                                               |                                       |
| 7   |                                                                                                                                                                                                                                                                               |                                       |
| 8   |                                                                                                                                                                                                                                                                               |                                       |
| 9   |                                                                                                                                                                                                                                                                               |                                       |
| 10  |                                                                                                                                                                                                                                                                               |                                       |
| 11  |                                                                                                                                                                                                                                                                               |                                       |
| 12  |                                                                                                                                                                                                                                                                               |                                       |
| 13  |                                                                                                                                                                                                                                                                               |                                       |
| 10  | 선택된 대여소의 ID에 따라 상세 정보(대여소 이름, 대여소 위치, 사용 가능 자전거 목록)를 조회한다. 사용 가능한 자전거가 있는 경우 즉시 대여가 가능하고, 없는 경우 예약 대기가 가능하다. 대여/예약 완료 시 문자 알림이 발송된다.                                                 | 대여소 상세정보 조회                  |
| 11  | 사용자 ID에 따라 사용자가 현재 대여 중인 자전거 목록의 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 조회한다. 자전거를 반납할 수 있고, 이때 식당 추천받기를 선택할 수 있다.                                                                        | 자전거 대여 정보 조회                 |
| 12  | 사용자 ID에 따라 예약 대기 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 조회한다. 각 예약건에 대하여 예약을 취소할 수 있다.                                                                                                                        | 자전거 예약 대기 정보 조회            |
| 22  | 회원은 요금 조회 화면에서 대여 시간과 요금을 조회할 수 있다.                                                                                                                                                                                                                  | 대여 시간 및 요금 조회                |
| 23  | 회원은 과거 자전거 대여 기록을 날짜별로 조회할 수 있다.                                                                                                                                                                                                                       | 이용 내역 조회                        |
| 24  | 회원은 과거 자전거 대여 기록을 대여소별로 정렬 기준을 변경하여 조회할 수 있다.                                                                                                                                                                                                | 이용 내역 조회 정렬 기준 변경         |
| 25  | 회원은 과거 자전거 대여 기록 중 특정 항목을 선택하여 삭제할 수 있다.                                                                                                                                                                                                          | 이용 내역 삭제                        |
| 26  | 관리자는 자전거 대여 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 반납 시간 기준 최근순으로 조회할 수 있다.                                                                                                                                        | 대여 정보 조회                        |
| 27  | 관리자는 자전거 대여 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 지역별로 정렬 기준을 변경하여 조회할 수 있다.                                                                                                                                    | 대여 정보 조회 정렬 기준 변경         |
| 28  | 관리자는 자전거 대여 금액 및 대여 횟수 통계를 조회할 수 있다.                                                                                                                                                                                                                 | 대여 금액 및 횟수 조회                |
| 29  | 관리자는 대여 금액 및 횟수 조회 기간을 최근 1주일, 1개월, 1년 단위로 선택하여 통계를 조회할 수 있다.                                                                                                                                                                          | 대여 금액 및 횟수 조회 기간 기준 변경 |
