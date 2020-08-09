---
title: "파일을 찾는 법 & 백그라운드 실행"
date: 2020-07-25T00:00:00-00:00
categories:
  - Linux
tags:
  - locate
  - find
  - Whereis
  - $PATH
  - Background

---

## 파일을 찾는 법

★ Locate

locate *.log : log의 확장자를 가진 모든 파일을 mlocate라는 DB 내에서 찾는다

★ Find

find / -name *.log : log의 확장자를 가진 모든 파일의 이름을 찾는다

★ Whereis

whereis ls : ls라는 명령어가 어느 디렉토리에 위치해 있는 지 알려준다

★ $PATH

echo $PATH : path 라는 환경변수에 담겨 있는 정보들이 보여진다

## 백그라운드 실행

★ Background

Ctrl + z : 실행중인 프로그램을 백그라운드로 보내는 단축키
             이 기능을 실행하면 명령어가 일시 정지됨

Fg : foreground의 약자, 백그라운드에 물러나 있다가 다시 포그라운드로 나타나게 됨
jobs : 백그라운드 작업들의 목록을 보여준다 

&가 명령어 뒤에 붙으면 명령어가 실행될 때 백그라운드로 실행된다

Ex)
ls -alR / > result.txt 2 > error.log & 
: ls -alR의 결과를 result.txt에 출력하고, 그 중 에러가 발생하면 error.log에 출력한다
