---
description: >-
  컴퓨터를 조작 하지 않고, 자동으로 특정시간에 무한매수법을 자동으로 매매 해줍니다. 여러사람, 여러계좌도 지원하며, 매매내역을
  메일,카카오톡으로 보내줍니다.
---

# Full Automatic Mode(완전 자동화) 설정 및 응용

## Full Automatic Mode(완전 자동화) 시연

****[**https://youtu.be/yj4iGCGOB3E**](https://youtu.be/yj4iGCGOB3E)****

## 필수사항

* 윈도우 자동로그인(암호 없이 로그인)



## **PC 자동 시작, Full Automatic Mode 설정(홈런타짜 님)**

{% embed url="https://cafe.naver.com/infinitebuying/7667" %}



## **여러사람 여러계좌 Full Automatic Mode 배치파일 설정 예시**

* 여러 사람, 여러 계좌  Full Automatic Mode 가능
* 프리장(17시)때 원화 주문 자동이 안되기 때문에, 매도(17시), 매수(19시 이후) 별도 주문 가능

kskyj\_RPA\_run.bat 예시 압축풀고 하세요. 또는 아래 내용 bat 로 만들면 됩니다. 해당 bat를 작업 스케쥴러에 등록하면 됩니다

{% file src="../.gitbook/assets/kskyj_RPA_run.zip" %}
kskyj\_RPA\_run
{% endfile %}

* **마지막 사용자를 빼고 나머지는 설정 > 일반/화면 > 종료시 윈도우 같이 종료 체크 해**
* **마지막 사용자는 설정 > 일반/화면 > 종료시 윈도우 같이 종료 체크**



### **#외화가 충분하거나 수동으로 자동원금설정 변경하는 경우, 또는 19시 이후에만 매매하는경 ( -A / --auto-mode 옵션)**

:: RPA경로로 이동

cd /d c:\kskyj\_RPA

:: 첫번째 사용자(윈도우 종료 하지 않을것)

&#x20;c:\kskyj\_RPA\kskyj\_RPA -A user\_data\_1.dat config\_1.ini



:: 영웅문 Process 종료&#x20;

wmic process where name='nfstarter.exe' delete&#x20;

wmic process where name='nfrunlite.exe' delete



:: 두번째 사용자 (윈도우 종료 해놓을것)

c:\kskyj\_RPA\kskyj\_RPA -A user\_data\_2.dat config\_2.ini



### #외화가 없거나 프리장때 수동으로 원화 주문설정을 피하는 방법(매도/매수 시간 분리)

**1.프리장때 매도 ( - AS / --auto-mode-sell 옵션)**

:: RPA경로로 이동

cd /d c:\kskyj\_RPA

:: 첫번째 사용자(윈도우 종료 하지 않을것)

&#x20;c:\kskyj\_RPA\kskyj\_RPA -AS user\_data\_1.dat config\_1.ini



:: 영웅문 Process 종료&#x20;

wmic process where name='nfstarter.exe' delete&#x20;

wmic process where name='nfrunlite.exe' delete



:: 두번째 사용자 (윈도우 종료 해놓을것)

c:\kskyj\_RPA\kskyj\_RPA -AS user\_data\_2.dat config\_2.ini





**2.본장에 매수 ( - AB / --auto-mode-buy 옵션)**

:: RPA경로로 이동

cd /d c:\kskyj\_RPA

:: 첫번째 사용자 (윈도우 종료 하지 않을것)

&#x20;c:\kskyj\_RPA\kskyj\_RPA -AB user\_data\_1.dat config\_1.ini



:: 영웅문 Process 종료&#x20;

wmic process where name='nfstarter.exe' delete&#x20;

wmic process where name='nfrunlite.exe' delete



:: 두번째 사용자 (윈도우 종료 해놓을것)

c:\kskyj\_RPA\kskyj\_RPA -AB user\_data\_2.dat config\_2.ini
