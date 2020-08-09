---
title: "아파치 웹서버 & SSH"
date: 2020-08-03T00:00:00-00:00
categories:
  - Linux
tags:
  - Apache
  - elinks
  - SSH
---

## 아파치 웹서버

★ Apache
`sudo service apache2 start` : apache2 서버 기동
`sudo service apache2 stop` : apache2 서버 끔

elinks : 웹 브라우저 켜서 접속하기
Ex) elinks htttp://127.0.0.1 : 자신의 IP 주소로 접속

apache2.conf : cd /etc 에 apache2에 대한 설정 파일이 저장되어 있음
대부분의 웹 서버는 사용자의 접속이 들어왔을 때 설정 파일의 내용을 참고해서 웹 브라우저에 표시함

## SSH

★ SSH
SSH를 통해 원격에 있는 컴퓨터를 제어 가능

`sudo apt-get intall openssh-server openssh-client` : Linux 환경에 openssh와 openclient 라는 이름의 서버를 다운로드
`sudo service ssh start` : ssh 서비스 기동
