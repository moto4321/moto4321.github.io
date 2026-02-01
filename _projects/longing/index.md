---
layout: post
title: 유학생 커뮤니티 Longing
description:
  학교의 관리 사각지대에 놓인 유학생 간 소통 부재를 해소하기 위해 기획, 개발된 서비스입니다.
  iOS app store에서 운영
skills:
  - Java
  - Springboot
  - JPA
  - Querydsl
  - Mariadb(AWS RDS)
  - S3 cloudfront
  - CodeDeploy

main-image: /image.png
---

---

<!-- # Header 1

Used for the title (already generated automatically at the top) -->

## 개발 기간

2024.12 ~ 2025.06

## 운영 기간

2025.06 ~ 2026.01

<!-- ### Header 3

Use this to have subsection if needed -->

<!-- ## Embedding images

### External images

{% include image-gallery.html images="https://live.staticflickr.com/65535/52821641477_d397e56bc4_k.jpg, https://live.staticflickr.com/65535/52822650673_f074b20d90_k.jpg" height="400"%}
<span style="font-size: 10px">"Starship Test Flight Mission" from https://www.flickr.com/photos/spacex/52821641477/</span>
You can put in multiple entries. All images will be at a fixed height in the same row. With smaller window, they will switch to columns. -->

### App images

{% include image-gallery.html images="IMG_0001.PNG, IMG_0003.PNG, IMG_0004.PNG, IMG_0005.PNG, IMG_9981.PNG, IMG_9982.PNG, IMG_9983.PNG, IMG_9984.PNG, IMG_9985.PNG, IMG_9986.PNG, IMG_9987.PNG, IMG_9988.PNG, IMG_9989.PNG, IMG_9990.PNG, IMG_9991.PNG, IMG_9992.PNG, IMG_9993.PNG, IMG_9994.PNG, IMG_9995.PNG, IMG_9996.PNG, IMG_9997.PNG, IMG_9999.PNG" height="400" %}

<br>

## 성능 개선

- s3 cloudfront 캐시처리로 이미지 조회 속도 개선, 보안 강화
- 이미지 업로드 presigned URL방식으로 클라이언트에 이미지 업로드 역할 위임하여 서버 부하 감소

## 개발 방식

- 도메인 중심 개발로 도메인 객체 데이터 처리는 각 도메인 클래스에 위임하여 객체 지향 설계 준수
- JUnit 테스트 코드 도입으로 기능 추가, 수정 시 회귀 버그 방지

## 인프라 구축

- launch template + codeDeploy를 사용한 블루/그린 무중단 배포 구축
- 서버 에러를 Slack 연동하여 알림 장애 대응 체계 구축
- 기능별 issue 생성 시 branch 자동 생성 github action 구축하여 배포 자동화 구축
- apple, google oauth2 기반 로그인 환경 구축
