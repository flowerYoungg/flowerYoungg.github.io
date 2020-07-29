---
title: "관리자와 일반 사용자 & 사용자의 추가"
date: 2020-07-29T00:00:00-00:00
categories:
  - Linux
tags:
  - 유저 권한
  - Linux
---

## 관리자와 일반 사용자

★ 관리자
Super / root user
`sudo passwd -u root` : u는 ulock의 약자
                         관리자 권한으로 변경하기 위해 잠금을 풂
`su - root` : 관리자 권한으로 변경


## 사용자의 추가
★ Add user
`sudo useradd -m '사용자'` : '사용자'의 디렉토리가 생성됨
`sudo passwd '사용자'` : '사용자'의 패스워드를 설정함
`sudo usermod -a -G sudo '사용자'` : '사용자'가 관리자 권한(sudo)을 사용 가능하게 만듦
`su - '사용자'` : '사용자'로 계정 변경
