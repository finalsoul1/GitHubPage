---
layout: post
title: VS Code - Code Helper CPU 점유율 100% 문제
tag: etc
---

징글징글한 vs code..

이번엔 vs code Code Helper가 cpu 점유율을 무지막지하게 먹는게 문제다.
(맥북이 막 울다 못해 죽을라 한다..)

일단 무엇이 문제인지 확인하자

```
$ ps aux | grep 11005
```

grep 뒤 숫자는 PID 인데, 각자 `활성상태보기`에서 문제의 Code Helper PID를 확인한 후 grep 뒤에 넣어서 확인하자.

나 같은 경우는 `tsserver log` 찍는게 문제라는데, 문제가 있어서 log를 찍는건지 log 찍는거 자체가 문제인건지..

아무튼 `tssever log`를 확인하는 방법은 

1. `settings.json`에서 
```
"typescript.tsserver.log": "verbose"
```
설정을 하시고  

2. vs code를 재시작 한다.  
3. 아무 코드를 수정하든지 해서 다시 cpu를 괴롭히자  
4. command palette에서 `> open tsserver log` 를 입력하면 파인더가 log파일이 있는 디렉토리를 열어준다.

참고로 나는 찬찬히 읽어보다가 빡쳐서 vscode에서 typescript 기능을 꺼버렸다. 난 typescript 안쓰거던..

vscode에서 기본으로 제공되는 익스텐션을 꺼버리거나 하고 싶을땐 익스텐션 탭에서 기본제공확장표시를 체크하면 목록을 확인할 수 있다.

아무튼 해결ㅋㅋㅋ 나중에 typescript 쓸 때 다시 생각하든지, 패치가 됐든지, 다른 코드에디터를 사용하든지 하자.

<a href="https://github.com/Microsoft/TypeScript/issues/26968" target="_sub">참고</a>

---