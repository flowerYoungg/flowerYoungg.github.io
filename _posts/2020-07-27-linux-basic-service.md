---
title: "항상 실행 & 정기적 실행"
date: 2020-07-27T00:00:00-00:00
categories:
  - Linux
tags:
  - daemon
  - service
  - CRON

---

## 항상 실행 (daemon, service)

★ daemon

항상 실행되고 있는 프로그램

★ Service

Ex) apache2라는 서비스 기동/정지
![image-left]({{ https://floweryoungg.github.io }}{{ linux-basic0727 }}/assets/images/apach2-service.jpg)

## 정기적으로 명령실행

★ CRON

crontab -e : nano 에디터가 실행됨(e는 edit)

 m h  dom mon dow command

	• M : minute

	• H : hour

	• Dom : day of month

	• Mon : month

	• Dow : day of week
