---
layout: post
title: Linux의 그림판인 kolourpaint. 그리고 스크린샷
tag: Linux
---

왜 이런 요상한 제목의 포스팅이 탄생 됐느냐..   
윈도우에서 스크린샷을 찍을 때 캡쳐도구를 이용하기도 하지만 나 같은 경우는 PrintScreen 키를 누르고 그림판에 붙여서 바로 간단하게 편집해 쓰곤 했다.

그런데 리눅스에서 스크린샷을 찍기위해 PrintScreen 키를 누르니 뭔가 찍히기는 하는데 붙여넣어야할 그림판이 보이지 않았다...

이러한 연유로 리눅스의 그림판인 kolourpaint를 소개한다(?)

- redhat계열(fedora, CentOS 등)

```terminal
# yum install kolourpaint
```

- devian계열(ubuntu, Linux Mint 등)

```terminal
# apt-get install kolourpaint4
```

![Kolorpaint](/public/img/Kolourpaint.png)

그냥 뭐.. 그림판이다.

근데 여기서 끝이 아니다. 붙여넣기가 안되더라..  
알고봤더니 사용자계정/사진 디렉토리로 바로 들어가 있었다.
필자는 CentOS7 설치 시에 환경그룹을 GNOME 데스크탑 환경에 체크하고 설치하니 스크린샷 프로그램이 자동으로 설치된 거였는데, 아마 GNOME은 다 같을거고 다른 데스크탑 환경을 설치하더라도 비슷할 거라 생각된다.

끗.