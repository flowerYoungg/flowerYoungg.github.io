---
title: "인터넷을 통한 서버 간 동기화 & 로그인 없이 로그인 하기"
date: 2020-08-05T00:00:00-00:00
categories:
  - Linux
tags:
  - rsync
  - ssh key
  - 로그인
---

## 인터넷을 통한 서버 간 동기화

★ rsync

인터넷을 통해서 컴퓨터와 컴퓨터의 파일을 동기화하는 방법(r : remote)
rsync -a src/ dest : src 폴더 안의 모든 파일을 dest 폴더로 동기화(복사) 한다

## 로그인 없이 로그인 하기

★ ssh key

`ssh -keygen` : 공개 키와 비공개 키 생성
Id_rsa : 비공개 키
Id_rsa.pub : 공개 키
`ssh-copy-id 로그인대상 컴퓨터의 ip` : authorized_keys에 공개키가 추가되어 로그인 가능하게 함

Encrypt : 암호화
Decrypt : 비암호화(복구화)
