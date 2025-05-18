# 메리츠 증권

## 0 메리츠 iMeritz 설치

#### 아래 사이트로 이동 하여 iMERITZ 설치

[https://home.imeritz.com/odermdia/OderMdiaDnldHts.do](https://home.imeritz.com/odermdia/OderMdiaDnldHts.do)

<figure><img src="../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

## 1 공동인증서 발급 또는 기존에 사용중인 인증서 가져오기

{% hint style="info" %}
공동인증서 무료로 발급해도 전혀 문제 없습니다.
{% endhint %}

{% hint style="info" %}
메리츠증권 자동매매는 현재 `공동인증서`만 지원합니다. `키움증권`의 공동인증서를 `메리츠증권에서 사용가능` 합니다.(타기관 인증서 등록 이용)
{% endhint %}

* 메리츠 증권 또는 타기관에서 발급한 공동인증서가 없을 경우, 아래 인증센터로 이동하여 공동인증서 발급
  * [https://home.imeritz.com/cust/athn/AthnCntr.do](https://home.imeritz.com/cust/athn/AthnCntr.do)
* 메리츠 증권은 신규 발급하면 클라우드 인증서로 발급 됩니다. 클라우드 인증서를 `인증서 내려받기`클릭하여 PC로 다운로드 하세요.
  * [https://home.imeritz.com/cust/athn/CloudAthnCntr.do](https://home.imeritz.com/cust/athn/CloudAthnCntr.do)
* 타기관(키움증권 등)에서 발급한 공동인증서가 있을 경우, 아래 타기관 인증서 등록
  * [https://home.imeritz.com/cust/athn/OthrPbcrReg.do](https://home.imeritz.com/cust/athn/OthrPbcrReg.do)

<figure><img src="../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

메리츠 HTS에서 로그인 클릭하면 위와 같이 인증서 목록이 보이면 됩니다.

{% hint style="success" %}
RPA에 설정 시 사용하는 인증서 순서는 맨위가 1번이고, 현재 선택된 것은 6번 입니다.
{% endhint %}

## 2 메리츠 로그인에서 마스터/인증서/PC저장 공동인증서 선택

* 마스터 선택
* 인증서 선택
* PC저장 공동인증서 선택

<figure><img src="../.gitbook/assets/image (104).png" alt=""><figcaption></figcaption></figure>

## 3 백신 예외 설정

{% embed url="https://fragilememor.gitbook.io/kskyj-rpa-kium/issue_solved/antivirus" %}

## 4 관리자 권한으로 실행처리

{% content-ref url="../issue_solved/administrator.md" %}
[administrator.md](../issue_solved/administrator.md)
{% endcontent-ref %}



## 5 사용자 계정 컨트롤 설정 변경

{% content-ref url="../issue_solved/uac.md" %}
[uac.md](../issue_solved/uac.md)
{% endcontent-ref %}



이제 세팅은 끝났습니다. 바탕화면의 지니RPA를 실행하고 아래 `퀵사용가이드`를 참고하세요.

![](<../.gitbook/assets/image (102) (1) (1).png>)

{% content-ref url="../quick_guide.md" %}
[quick\_guide.md](../quick_guide.md)
{% endcontent-ref %}
