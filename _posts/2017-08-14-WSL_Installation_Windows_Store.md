---
title: "WSL 설치 (Windows Store버전)"
date: 2017-08-14 08:26:28
categories: 01_Install 
tags: WSL
---

# WSL 설치 (Windows Store통해)
@(OpenCV_Python)[01_install WSL]

본 문서는 microsoft store을 이용하여 WSL설치하는 것을 다룸.

lxrun를 이용하는 방법은 다음 페이지 참고.

### **Windows PowerShell**을 *관리자 권한*으로 실행.

* `Window키 + R` 을 누르면 “실행” 이 뜸.
* 거기에 powershell 이라고 기재하고 Ctrl+Shift+Enter 입력시 PowerShell이 관리자 권한으로 수행됨.
* 다음 명령어를 복사하여 powershell에서 실행.
```Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux```
* 이후 리부팅 필요함.

![O1_Install_WSL_01](https://docs.google.com/drawings/d/e/2PACX-1vR-hieWUOQhIwwD9cW4SC9q4bBOV3X8u2pn92vCB-4f8E75o8NcPTRfZLJrpAF8-kUDNtBZu2-tTDDN/pub?w=549&h=100)

---

### 윈도우 버전이 낮을 시 다음과 같은 오류 발생시

![01_Install_WSL_02](https://docs.google.com/drawings/d/e/2PACX-1vQJlL8_YTTAthPa-hfc6rFIiIf0rH-xlcHWxJ6cMubCwFJ049FRcac__yTxm3K5kCxuUzgBFAhNxKgD/pub?w=607&h=100)

* bme계정 팀드라이브 / MMMIL / Setup / OS / Windows10Upgrade9252.exe 를 실행하여 윈도우 업데이트 진행 (업데이트 진행 후 구글Chrome 사용에 문제가 발생하여 레지스트리 작업이 필요함)
	* sol : (https://dsaint31x.github.io/Blog/etc/2018/07/20/Etc-Chrome-Cryptographic.html)
* Windows 10 x64 1709(Fall Creators 업데이트) 이상의 버전으로 업데이트 해도 됨.
	* download : (https://www.microsoft.com/ko-kr/software-download/windows10)

### microsoft store 에서  Ubuntu 받기.

* 다운로드 받은후 아래 화면에서 실행을 수행.
![01_Install_WSL_03](https://docs.google.com/drawings/d/e/2PACX-1vRLfevfnaGJxFZcu58fvyd7RTi_IPR8Fyznd7IEs1fhmKIAxApQAdx6mY7-iewBNeNoz1ZJtBCnttOP/pub?w=376&h=224)
* 실행후 설치 완료된 화면
![01_Install_WSL_04](https://docs.google.com/drawings/d/e/2PACX-1vTceJvUa6-0g1O2GgBB4EHg9wDj6uWKK1dyjraNgFbMSOSSj1VU6eooYsweFhibSgb-jH1GaaRSBpK6/pub?w=531&h=244)
