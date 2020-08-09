---
title: "권한 & 그룹"
date: 2020-07-30T00:00:00-00:00
categories:
  - Linux
tags:
  - Permission
  - chmod
  - group
---

## 권한

★ Permission

File & Directory 에 대한 권한을 지정함

Read(r) / Write(w) / Execute(x) 의 권한 지정

*-rw-rw-r--(access mode)*

: 첫 번째 -rw 는 owner, 두 번째 -rw는 group, r--는 other의 권한을 지칭


★ 권한을 변경하는 방법 : chmod

*chmod* : change mode

chmod / 어떻게 모드를 바꿀 것인가 / 모드를 바꿀 대상

Ex)

 `chmod / o+r / test.txt` : 모든 사람(other)이 test.txt 를 읽을 수 있는(read) 권한을 부여

 `chmod / u-r / test.txt` : 소유자(user)가 test.txt 를 읽을 수 있는(read) 권한을 제거

 `chmod -R o+w perm` : perm 이라는 디렉토리 안의 모든 디렉토리에 대해서 쓰기 권한을 부여



## 그룹

★ group

파일과 디렉토리를 여러 사용자들이 공동으로 관리 할 수 있는 방법

groupadd 그룹이름 : 새로운 그룹을 만들 때
