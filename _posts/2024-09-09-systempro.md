---
layout: single
title: "Computer systems"
categories: "시스템프로그래밍"
---

## 컴퓨터 시스템의 계층도

<ol>
  <li>Software 계층</li>
  <ul>
    <li style="font-size:15px;">application programs</li>
    <li style="font-size:15px;">Operating System</li>
  </ul>
  <li>Hardware 계층</li>
  <ul>
    <li style="font-size:15px;">processor, main memory, i/o devices</li>
  </ul>
</ol>


## 하드웨어 구성요소
<ol>
  <li>버스(buses)</li>
  <ul>
    <li style="font-size:15px;">구성요소간의 정보교환 통로</li>
    <li style="font-size:15px;">하나의 하드웨어에서 다른 하드웨어로 데이터를 실어 나르는 노선<li>
    <li style="font-size:15px;">종류: 입출력버스, 시스템버스</li>
  </ul>
  <li>입출력 장치(i/o devices)</li>
  <li>주기억장치(main memory)</li>
  <li>캐쉬(cache memory)</li>
  <li>중앙처리장치(cpu)</li>
  <ul>
    <li style="font-size:15px;">산술논리연산장치(ALU)<li>
    <li style="font-size:15px;">제어장치: control unit<li>
    <li style="font-size:15px;">레지스터<li>
    <ul>
      <li style="font-size:15px;">프로그램 카운터(pc)<li>
      <li style="font-size:15px;">상태 레지스터<li>
      <li style="font-size:15px;">메모리 주소 레지스터<li>
      <li style="font-size:15px;">메모리 데이터 레지스터<li>
      <li style="font-size:15px;">명령 레지스터, instruction pointer, IP<li>
      <li style="font-size:15px;">범용 레지스터, general-purpose register<li>
    </ul>
    <li style="font-size:15px;">주요기능<li>
    <ul>
      <li style="font-size:15px;">기억장치로부터 명령/데이터 호출 및 저장<li>
      <li style="font-size:15px;">명령의 해석 : 제어장치<li>
      <li style="font-size:15px;">명령의 실행 : ALU<li>
      <li style="font-size:15px;">입출력 연산 : I/O<li>
    </ul>
    <li style="font-size:15px;">명령 주기(Instruction cycle) *중요<li>
    <ul>
      <li style="font-size:15px;">인출 fetch : PC에 의거하여 명령어를 가져옴<li>
      <li style="font-size:15px;">해독 decode : 명령어를 해석하여 제어 신호 생성<li>
      <li style="font-size:15px;">실행 execution : 가져온 명령어를 실행<li>
      <li style="font-size:15px;">결과저장 store : 실행 결과를 저장<li>
    </ul>
  </ul>
</ol>

## 운영체제
<ul>
  <li>응용프로그램이 하드웨어를 효율적으로 사용할 수 있도록 도와주는 프로그램</li>
  <ul>
    <li style="font-size:15px;">하드웨어 추상화 Hardware Abstraction<li>
    <li style="font-size:15px;">시스템 인터페이스 추상화<li>
  </ul>
  <li>관리대상</li>
  <ul>
    <li style="font-size:15px;">프로세스<li>
    <li style="font-size:15px;">메모리<li>
    <li style="font-size:15px;">입출력장치<li>
    <li style="font-size:15px;">소프트웨어 자원(파일시스템, 라이브러리, 유틸리티)<li>
  </ul>
  <li>컴파일 과정</li>
  <ul>
    <li style="font-size:15px;">소스코드가 전처리기를 거쳐 modified source program생성<li>
    <li style="font-size:15px;">modified source program이 컴파일러를 거쳐 어셈블리코드로 변환<li>
    <li style="font-size:15px;">어셈블리코드가 어셈블러를 거쳐 기계어로 변환<li>
    <li style="font-size:15px;">기계어가 생성되면, linker를 호출하여 실행가능한 오브젝트 생성<li>
  </ul>
</ul>