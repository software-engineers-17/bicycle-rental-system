# bicycle-rental-system

공유 자전거 대여 시스템

## Requirement List

| No. | Requirement | Use Case |
| --- | ----------- | -------- |
| 1 | System users can register for membership. The required information for membership registration includes ID, password, phone number, payment method, and preferred bike type (standard/electric). The administrator can log in with the given ID (admin) and password (admin). | Regist Membership |
| 2 | Members can withdraw their membership at any time. Upon withdrawal, all user privileges and data are deleted. | Withdrawal Membership |
| 3 | Administrators and members can log in to the system using their ID and password. Upon logout, the system connection is terminated. | Login/ Logout |
| 4 | | |
| 5 | | |
| 6 | | |
| 7 | | |
| 8 | | |
| 9 | | |
| 10 | | |
| 11 | | |
| 12 | | |
| 13 | | |
| 14 | | |
| 15 | | |
| 16 | | |
| 17 | | |
| 18 | | |
| 19 | | |
| 20 | | |
| 21 | | |
| 22 | | |
| 23 | 회원은 자전거 반납 시 결제 시스템이 호출되어 사용 시간에 따라 요금이 자동 결제된다. | 자전거 반납 |
| 24 | 회원은 요금 조회 화면에서 대여 시간과 요금을 조회할 수 있다. | 대여 시간 및 요금 조회 |
| 25 | 회원은 과거 자전거 대여 기록을 날짜별로 조회할 수 있다. | 이용 내역 조회 |
| 26 | 회원은 과거 자전거 대여 기록을 대여소별로 정렬 기준을 변경하여 조회할 수 있다. | 이용 내역 조회 정렬 기준 변경 |
| 27 | 회원은 과거 자전거 대여 기록 중 특정 항목을 선택하여 삭제할 수 있다. | 이용 내역 삭제 |
| 28 | 관리자는 자전거 대여 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 반납 시간 기준 최근순으로 조회할 수 있다. | 대여 정보 조회 |
| 29 | 관리자는 자전거 대여 정보(대여소 이름, 대여소 위치, 자전거 ID, 자전거 제품명, 자전거 유형)를 지역별로 정렬 기준을 변경하여 조회할 수 있다. | 대여 정보 조회 정렬 기준 변경 |
| 30 | 관리자는 자전거 대여 금액 및 대여 횟수 통계를 조회할 수 있다. | 대여 금액 및 횟수 조회 |
| 31 | 관리자는 대여 금액 및 횟수 조회 기간을 최근 1주일, 1개월, 1년 단위로 선택하여 통계를 조회할 수 있다. | 대여 금액 및 횟수 조회 기간 기준 변경 |

## Use Case Description

#### Register Membership Description

| Actor | System |
| ----- | ------ |
| the user selects the membership registration menu | |
| | The system presents membership registration form |
| The user enters the required information (ID, password, phone number, payment method, preferred bike type - standard/electric)1 and requests registration. | |
| | The system validates the entered information and processes the registration. |
| | The system displays a message confirming successful membership registration. |
| | If the entered information is invalid (e.g., incorrect format, missing required field), the system displays an error message and prompts for re-entry. |
| | If the entered ID is already in use, the system displays a message indicating ID duplication and prompts the user to enter a different ID. |

#### Membership Withdrawal

| Actor | System |
| ----- | ------ |
| The member selects the membership withdrawal function (e.g., from a profile or settings menu). | |
| | The system displays a confirmation message and outlines the withdrawal procedure. |
| The member confirms the decision to withdraw. | |
| | The system deletes all the member's user privileges and associated data. |
| | The system displays a message confirming successful membership withdrawal. |

#### Login

| Actor | System |
| ----- | ------ |
| The administrator or member enters their ID and password on the login screen and requests to log i | |
| | The system verifies the entered ID and password against registered user creden |
| | If authentication is successful, the system grants access to the user and navigates to the main system in |
| If the entered ID or password does not match any registered credentials, the system displays an error message indicating incorrect login details. in details. | |

#### Logout

| Actor | System |
| ----- | ------ |
| The administrator or member selects the logout option (e.g., from a menu or button). | |
| | The system terminates the user's current session and system connection. |
| | The system typically redirects the user to the login screen. |