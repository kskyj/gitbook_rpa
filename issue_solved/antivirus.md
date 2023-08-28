# 백신 예외 설정(사용하는 백신에 따라 다름)

RPA같은 자동화 도구는 백신에서 바이러스로 오진하는 경우가 있기 때문에 예외를 해야 합니다.&#x20;

{% hint style="info" %}
아래 설명은 윈도우10 기본 백신에 대한 설명이며 다른 백신의 경우 각 백신 설정에 따라 다릅니다.
{% endhint %}

### 바이러스 오진 확인 방법

1. **윈도우 > 설정 > 업데이트 및 보안 또는 개인정보 및 보안(윈도우 마다 메뉴 다름) > 보안 선택**

![](<../.gitbook/assets/image (80).png>)

2. 보호 기록 선택 하면 차단된 항목 확인이 가능합니다.

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>



### 바이러스  및 위협방지 제외

1. **윈도우 > 설정 > 업데이트 및 보안 또는 개인정보 및 보안 > 보안 선택**
2. **바이러스 위협 및 방지 > 바이러스 및 위협 방지 설정**

![](<../.gitbook/assets/image (81).png>)

![](<../.gitbook/assets/image (82).png>)



3. **제외 > 제외 추가 또는 제거**

![](<../.gitbook/assets/image (83).png>)



4. **제외사항 추가 > 폴더 선택 > RPA폴더 지정하고 \[폴더 선택]**

![](<../.gitbook/assets/image (84).png>)

![](<../.gitbook/assets/image (85).png>)

아래 폴더들을 지정합니다.

* C:\kskyj\_RPA
* C:\kskyj\_RPA\download
* 인터넷 브라우저파일 다운로드 경로(최초 설치시 kskyj\_RPA\_vxxxx\_Setup.exe 파일이 지워 지는 경우 설정하세요) > 보안상 안전하지 않기 때문에 RPA 설치후 해당 경로는 제외에서 제거하세요.



5. **제외 > 파일 선택**

![](<../.gitbook/assets/image (19).png>)

아래 파일을 지정합니다.

* **C:\kskyj\_RPA.exe**







### 앱 및 브라우저 컨트롤 예외

{% hint style="danger" %}
바이러스 및 위협방지 제외를 적용해도 안되는 경우 설정하세요.
{% endhint %}

1. **윈도우 > 설정 > 업데이트 및 보안 또는 개인정보 및 보안 > 보안 선택**
2. **앱 및 브라우저 컨트롤 선택**

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

3. **Expoit Protection 설정 선택**

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

4. **프로그램 설정 > + 프로그램을 추가해 사용자 지정 > 프로그램 이름별 추가**

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>



5. kskyj\_RPA.exe 입력 후 추가

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>



6. 모든 항목 시스템 설정 재정의 클릭 및 끔 선택 > 적

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

