---
layout: post
title: Linux의 주요 Command
tag: Linux
---

- 파일 및 디렉토리 관리 명령어

```terminal
pwd, realpath : 현재 작업 디렉토리 위치 확인 
```

```terminal
cd : 작업 디렉토리 이동
cd / : 루트 디렉토리로 이동
cd .. : 한 단계 상위 디렉토리로 이동
cd ~ : 현재 사용자의 홈 디렉토리로 이동
cd - : 바로 전 디렉토리로 이동
```

```terminal
ls : 파일목록 보기
-a : 숨김 파일 포함
-l : 상세 보기
-t : 변경시간 기준 정렬
```
>``ls -al`` 이런식으로 옵션을 겹칠 수 있다.  
풀네임으로 옵션을 줄때는 `--help` 이런식으로 -- 두개를 붙인다

```terminal
tree : 파일 및 디렉토리 트리 보기
```

tree는 따로 설치해야 하는 경우도 있다.

```terminal
# yum install tree
```

`# tree -d` 하면 아래처럼 blog/ 아래 디렉토리만 출력한다  
![tree](/public/img/ls-tree.png)


```terminal
touch : 파일 생성, 날짜 시간정보 변경
mkdir : 디렉토리 생성
```

```terminal
cp : 파일 및 디렉토리 복사
-d : 링크를 보존
-p : 소유자, 그룹, 권한, 시간정보들이 그대로 복사
-R/-r : 모든 서브 디렉토리, 하위경로와 파일들 모두 복사
-a : 복사되는 파일의 구성과 속성 모두 복사 -dpR과 같은 옵션
```

```terminal
mv : 파일 및 디렉토리 이동
rename : 파일 및 디렉토리 이름 변경
```

```terminal
rm : 파일 및 디렉토리 삭제
-r : 디렉토리 삭제할 때 붙인다, 디렉토리에 포함된 파일도 함께 삭제한다.
```
> -r 만 붙이면 삭제할 때마다 삭제여부를 묻는다  
> `rm -rf` 하면 걍 싹 지움.

```terminal
rmdir : 디렉토리 삭제
find : 파일 및 디렉토리 검색
du : 파일 및 디렉토리 용량 확인
file : 파일 종류 확인
stat : 파일 및 파일 시스템 상태 표시
tar : 파일 및 디렉토리 묶기
gzip : 파일 압축
bzip2 : 파일 압축
xz : 파일 압축
chmod : 파일 권한 바꾸기
chown : 파일 소유자 변경
chgrp : 소유 그룹 변경
umask : 파일 퍼미션 마스크
```

---