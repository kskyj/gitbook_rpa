# 기본매도 비율 설정, 윈도우종료 등 config.ini 설정

특별한 경우가 아니면 수정하실 필요 없습니다.&#x20;

**kskyj RPA 프로그램 키고 변경하면 반영 안됩니다. 프로그램 시작전에 파일을 메모장등으로 열어서 변경하고, 저장 후 프로그램을 시작해야 반영됩니다.**

kskyj RPA 프로그램  내 settings 폴더안에 있으며 기본경로는  C:\kskyj\_RPA\settings\conf.ini 입니다.

![](<../../.gitbook/assets/image (61).png>)

아래 언급한것 외에 다른것 변경시 정상적으로 동작하지 않을 수 있습니다.

*   ticker : 계좌 잔고에 보유하고 있는 자동으로 가져올 종목 설정

    * 종목을 안가져오는 경우 : 해당 내용에 종목 추가
    * 자동으로 안가져오길 원하는 종목이 있을 경우 : 해당 내용에서 종목 제거


*   default\_sell\_ratio : 전체 기본 매도 비율 설정(매도 버튼에 표시됨)

    * 기본값 : 10.17%
    * 9% \~ 20% 범위를 넘어 설 경우 10.17% 로 동작


* default\_sell\_split\_ratio : 전체 기본 분할 매도 비율 설정(분할매도 옵션에 표시됨)
  * 기본값 : 5.17%
  *   4% \~ 11% 범위를 넘어 설 경우 5.17%로 동작


* sell\_split\_mode : RPA 실행시 기본 분할 매도 사용 여부 설정(RPA 실행시 기본값이며 체크박스에 따라 수행됨)
  * sell\_split\_mode = true : 50% 진행시 분할 매도 수행
  *   sell\_split\_mode = false : 50% 진행시 분할 매도 하지 않음


*   vertical\_size : 종목 개수 조절로 2가지 모드만 제공(1.2.2 부터 자동으로 감지하여 변경됨)

    * vertical\_size = default : 16개
    * vertical\_size = max : 28개


*   exit\_with\_window : 종료시 윈도우 종료 여부 설정(풀오토모드 동작시에도 동작)

    * exit\_with\_window = true : 종료시 윈도우 종료 확인
    * exit\_with\_window = false : 종료시 윈도우 종료 안내


*   user : 화면 상단에 표시되는 메시지


*   custom\_color : 상단 및 하단 색상 변경

    * HTML 컬러코드 사용 #E6E6E6


*   certificate\_save : 공동인증서 비밀번호 암호화 저장으로 사용시 주의 요망

    * certificate\_save = true : 공동인증서 비밀번호 암호화 형태로 저장
    * certificate\_save = false(기본값) : 공동인증서 비밀번호 저장하지 않음


*   before\_opening\_test : 휴일 개장전 테스트용 모드로 주문 에러 메시지 무시

    * before\_opening\_test = true : 휴일 개장전 테스트용 모드로 동작
    * before\_opening\_test = false(기본값) : 일반 모드로 동작


*   default\_dealy : 매매 기본 딜레이값으로 낮을경우 매매 속도 상승, 노트북 느린네트워크에서 매매실패시 변경하지 말것

    * 기본값 : 0.5
    * 최소값 0 : 가장 빠름


*   hts\_wait\_dealy : 영웅문 Global 실행 대기 시간 설정

    * 기본값 : 25(초)


*   loc\_sell : 매도시 LOC매도 진행(LOC매도 아는분만 쓰세요)

    * loc\_sell = true : 모든 종목 매도시 LOC매도로 진행
    * loc\_sell = false(기본값) : 지정가 매도로 진행


*   hts\_run\_check\_popup : 영웅문 프로세스 감지 경고 표시(v1.5.1 삭제)

    * hts\_run\_check\_popup = true(기본값) : 영웅문 프로세스 감지 못했을 경우 경고&#x20;
    * hts\_run\_check\_popup = false : 영웅문 프로세스 감지 못해도 경고 나오지 않음


* auto\_update\_check : 자동업데이트
  * auto\_update\_check = true(기본값) : kskyj RPA 실행시 최신버젼 감지
  * auto\_update\_check = false : kskyj RPA 실행시 최신버젼 감지 안함

&#x20;
