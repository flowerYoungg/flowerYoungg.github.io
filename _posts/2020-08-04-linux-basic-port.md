---
title: "포트 & 도메인"
date: 2020-08-04T00:00:00-00:00
categories:
  - Linux
tags:
  - Port
  - Port forwarding
  - DNS
---

## 포트

★ Port

네트워크를 통해 적절한 어플리케이션을 실행시키기 위한 것

0~1024 : well known port 많이 쓰이는 유명한 포트 번호

★ Port forwarding

`ip route` :  Default gateway 의 IP

`curl http://ipinfo.io/ip` : 자신이 접속한 컴퓨터가 어떠한 공개 IP를 사용하고 있는지 습득 가능

Ex)
공개 IP주소 : 9000 에 사용자가 접속한다고 하면, 9000번의 포트가 지정되어 있는

개인 IP주소 :  ~port번호 로 포워딩 하게 되어 있음

## 도메인

★ DNS

Domain Name System Server

Google.com 을 검색창에 입력한다면 .com 을 담당하는 DNS 서버가 무엇인지
Root DNS Server에 물어보고, Root DNS Server는 그 대답을 DNS 서버에 돌려줌
