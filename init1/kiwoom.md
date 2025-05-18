# 키움 증권

## 0 영웅문 Global 로그인 설치

#### 아래 사이트로 이동 하여 영웅문Global 설치

{% embed url="https://download.kiwoom.com/herog_custom/KiwoomGlobalSetup.exe" %}
클릭해서 다운로드 후 설치
{% endembed %}

![](<../.gitbook/assets/image (31).png>)

## 1 간편인증서/공동인증서 발급 또는 기존에 사용중인 인증서 가져오기

{% hint style="info" %}
공동인증서 무료로 발급해도 전혀 문제 없습니다.
{% endhint %}

{% hint style="info" %}
키움증권 자동매매는 현재 `간편인증`과 `공동인증서`를 지원합니다. 특별한 사유가 없는 경우 보안이 더 좋은 `간편인증` 사용을 권장합니다.
{% endhint %}

* 간편인증 [https://www1.kiwoom.com/h/customer/cert/VCertCenterSimpleAuthInfoView?dummyVal=0](https://www1.kiwoom.com/h/customer/cert/VCertCenterSimpleAuthInfoView?dummyVal=0)
* 공동인증서 [https://www1.kiwoom.com/h/customer/cert/VPublicCertCenterView?dummyVal=0](https://www1.kiwoom.com/h/customer/cert/VPublicCertCenterView?dummyVal=0)
  * 키움 증권 또는 타기관에서 발급한 공동인증서가 없을 경우, 인증센터로 이동하여 공동인증서 발급
  * 타기관에서 발급한 공동인증서가 있을 경우, 인증센터에서 인증서 등록

## 2 영웅문 로그인에서 간편인증/공동인증서 선택 및 매번 입력 해제

* 간편인증 또는 공동인증서 선택(ID, 모의투자 선택 하면 안됨)
* 체크 : XX인증 자동 팝업
* 체크해제 : XX인증 매번 입력

![](<../.gitbook/assets/image (102).png>)

## 3 영웅문 Global 기본환경설정, 계좌번호 저장 및 보안설정

#### **1. 기능 > 종합환경설정 이동**

\*\*\*\*![](https://gblobscdn.gitbook.com/assets%2F-MZ-Y7H8lCWI22Yo_bhV%2F-MZTEoY7sSwRc_THQwd0%2F-MZTGyXVtpwwo9AEgjRl%2Fimage.png?alt=media\&token=3a700c3a-0ad7-4b80-83a9-74e623036405)

#### **2. 기본환경**

{% hint style="warning" %}
아래 설정을 하지 않는 경우 SOXL등과 같이 고유 Ticker가 아닌경우 매매 주문검증 실패가 발생합니다.
{% endhint %}

* 검색창에 종목리스트보기
  * \[체크해제] 종목코드 검색 시 엔터키로 종목리스트 보기
  * \[체크] 중간어, 종목명 검색 기능 사용
* 주문, 잔고설정
  * \[체크해제] 주문버튼 Enter키/Space키 주문 사용안함

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

#### **3. 보안설정으로 이동후 계좌 비밀번호 입력후 아래 설정후 확인**

* 계좌별 비밀번호 입력(회색 네모부분 옆)
* \[체크] 다음 접속시에도 저장된 비밀번호 유지하여 계속 사용
* \[체크해제] 멀티로그인(동시접속) 팝업알림 해제
* \[체크해제] 메모리 보안 적용 해제

![](<../.gitbook/assets/image (104) (2) (1) (1).png>)

## 4 백신 예외 설정

{% embed url="https://fragilememor.gitbook.io/kskyj-rpa-kium/issue_solved/antivirus" %}

## 5 관리자 권한으로 실행처리

{% content-ref url="../issue_solved/administrator.md" %}
[administrator.md](../issue_solved/administrator.md)
{% endcontent-ref %}

## 6 사용자 계정 컨트롤 설정 변경

{% content-ref url="../issue_solved/uac.md" %}
[uac.md](../issue_solved/uac.md)
{% endcontent-ref %}

이제 세팅은 끝났습니다. 바탕화면의 지니RPA를 실행하고 아래 `퀵사용가이드`를 참고하세요.

![](<../.gitbook/assets/image (102) (1) (1).png>)

{% content-ref url="../quick_guide.md" %}
[quick\_guide.md](../quick_guide.md)
{% endcontent-ref %}
