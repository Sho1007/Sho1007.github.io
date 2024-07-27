---
title: "[혼공 학습단 12기] 혼공컴운 3주차"
category:
    - HonGong
tag:
    - Computer Structure
    - Operating System
toc: true
toc_sticky: true
date: 2024-07-21
last-modified-at: 2024-07-21
---
![image](../../assets/images/HonGongCSOS.jpg)


## 진도 : Chapter 06 ~ 08

## 기본 숙제   
1. **p.185의 확인 문제 3번**   
* 주로 캐시 메모리로 활용됩니다. `SRAM`
* 주로 주기억장치로 활용됩니다. `DRAM`
* 대용량화하기 유리합니다. `DRAM`
* 집적도가 상대적으로 낮습니다. `SRAM`
2. **p. 205의 확인 문제 1번**   
레지스터   
캐시 메모리   
메모리   
보조기억장치


## 추가 숙제
**Ch.07(07-2) RAID의 정의와 종류를 간단히 정리해 보기**   
### RAID
> 데이터의 안전성 혹은 높은 성능을 위해 여러 개의 물리적 보조기억장치를 마치 하나의 논리적 보조기억장치처럼 사용하는 기술을 의미합니다.

* RAID0 : 여러 개의 보조기억장치에 데이터를 단순히 나누어 저장하는 구성 방식
* RAID1 : RAID0의 복사본을 만드는 방식   
(RAID0에서 A1, A2, A3, A4 이렇게 4개에 나눠서 저장했다면, RAID1에서는 A1, A2 로 나눠서 저장하고 이것을 복사하여 복사본 A1, A2가 존재한다)
* RAID4 : RAID1처럼 완전 복사본을 만드는 대신 오류 검출 위해 `패리티 비트`를 저장하는 장치를 두는 구성 방식
* RAID5 : RAID4에서 존재하던 패리티 정보를 분산하여 저장하는 방식으로, RAID4의 문제인 병목 현상을 해소
* RAID6 : RAID5와 기본적인 구성은 같으나, 서로 다른 패리티 정보 2개를 두는 방식. 새로운 정보를 저장할 때마다 함께 저장할 패리티가 두 개이므로, RAID5보다 느리지만, 패리티 비트 중 하나가 손상되더라도 다른 하나를 통해 복구할 수 있으므로 안전