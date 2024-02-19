이씨와 함께하는 김씨들의 팀 프로젝트
=====================
 1 . 프로젝트 프로그램 구현 기능
=====================


사용자 관리 기능

-0- 로그인 환경 구현.[LoginConfiguration]
admin 은 따로 구현
각 객체 아이디,패스워드,접근 권한 설정

-1- 사용자 등록[UserRegistration]
총괄 임원
하부 관리자 팀장급 과장급 등등
직원
사용자를 등록.

-2- 사용자 (출근) / (퇴근)[UserCommute]
등록된 사용자가 시스템에 로그인하고 로그아웃할 수 있는 기능
 e x )
해당 기능은 Date 를 기반으로 출근일(평일) 의 논리값을 false 혹은 'N' 를 기본값으로 함.
(출근) 할 경우 논라값을 true 혹은 'Y' 로 전환해서 Date 따로 저장. 
(퇴근) 할 경우 논리값으 false 혹은 'N' 으로 전환해서 Date 따로 저장.
해당 기능은 로그인 로그 아웃을 따로 만들지 않고 (출근) 할때 값이 반대가 되도록 해도 된다.
Date 활용해서 출근 시간과 퇴근 시간 체크 가능하도록 하고
#근태 기록 코드 세분화 지각,조퇴,병가,반차,월차 등등 추가

-3-.  페널티 기능 목록 추가(감봉, 만근수당 제외, 사유서 제출 등등) [Penalty]
    # 각 개개인이 열람가능.

-4- 근태 우수 사원 목록 추가[BestEmployeesAward]
    # 순위에 따라 상여금 or 휴가 or 등등

-5- 출근 체크[AttendanceCheck] 
사용자가 현재 출근 했는지 여부를 체크할 수 있는 기능.
e x )
해당 기능은 관리 프로그램을 통해 해당 근무자의 (PK값)으로 설정 해서 
위의 로그인 여부 호출 해야함.( true 혹은 'Y' 면' 적어도 출근은 한상태.)

-6-출근 기록 조회[AttendanceRecodeCheck]
특정 날짜 및 사용자에 대한 출근 기록을 조회할 수 있는 기능
e x )
전체 데이터베이스 에서 출근의 기록이 월별로 저장되도록 저장. 

-7-출근 통계[AllInformationProvision]
출근률, 지각 횟수 등의 통계 정보를 제공하는 기능
e x )
저장된 데이터 베이스에서 출근/결근/조퇴/기타 등등 지정한 Date로 조회 가능하게 통계 자료 따로 구현 (월별, 연도별, 등등)

-8-일정 또는 이벤트 생성[MakeEvent]
새로운 일정 또는 이벤트를 생성하고 관리할 수 있는 기능
e x ) 
8-1. 결재 시스템 목록 추가 (기안작성,반차,휴가일정 등등)[ApprovalSystem]

-9-사용자 권한 관리[UserAuthorizationManagement]
관리자가 다른 사용자에 대한 권한을 관리할 수 있는 기능

-10-데이터 관리[DataManagement]-SQL
출석 기록 및 사용자 정보를 관리할 수 있는 기능

-11-출근/퇴근 알림[InformedCommute]
등록된 사용자에게 출석 여부에 관한 알림을 전송할 수 있는 기능
== 미구현

-12-일정 알림[InformedDate]
수업 또는 이벤트의 시작 전에 사용자에게 알림을 전송할 수 있는 기능
== 미구현

-13-접근 제어[AccessControl]
사용자가 권한 없이 시스템에 접근하는 것을 방지하는 기능


-14-사용성 개선[ImprovedUtilization]
사용자 경험을 향상시키는 기능 (인터페이스 디자인, 사용 편의성 등)


 




