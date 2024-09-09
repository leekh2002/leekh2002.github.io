---
layout: single
title: "Computer Abstractions & Technology-1"
categories: "컴퓨터구조"
---

## Classes of Computers

<ol>
  <li>Personal computersㄹ</li>
  <ul>
    <li style="font-size:15px;">범용적으로 사용,다양한 소프트웨어</li>
    <li style="font-size:15px;">가격, 성능은 반비례관계(가성비 고려)</li>
  </ul>
  <li>Server computers</li>
  <ul>
    <li style="font-size:15px;">네트워크 기반</li>
    <li style="font-size:15px;">대용량, 성능, 안정성을 요구</li>
    <li style="font-size:15px;">소규모 서버부터 빌딩 크기에 아우르는 넓은 범위</li>
  </ul>
  <li>Supercomputers</li>
  <ul>
    <li style="font-size:15px;">과학적, 엔지니어링 의 고급화된 계산</li>
    <li style="font-size:15px;">가장 높은 성능을 자랑하지만 컴퓨터 시장의 작은 부분을 차지</li>
  </ul>
  <li>Embedded computers</li>
  <ul>
    <li style="font-size:15px;">시스템의 구성요소로 숨겨져있음</li>
    <li style="font-size:15px;">엄격한 전력/성능/비용 제약조건</li>
  </ul>
</ol>

## 성능에 영향을 미치는 요소

<ol>
  <li>Algorithm</li>
  <ul>
    <li style="font-size:15px;">수행되는 연산자의 수 결정</li>
  </ul>
  <li>Programming language, compiler, architecture</li>
  <ul>
    <li style="font-size:15px;">작업당 수행되는 machine instructions 수 결정</li>
  </ul>
  <li>Processor and memory system</li>
  <ul>
    <li style="font-size:15px;">실행되는 명령어가 얼마나 빠른지 결정</li>
  </ul>
  <li>I/O system (OS포함)</li>
  <ul>
    <li style="font-size:15px;">입출력 동작이 얼마나 빠른지 결정</li>
  </ul>
</ol>

## Seven Great Ideas in Computer Architecture

<ol>
  <li>추상화로 설계를 단순화</li>
  <li>공통적인 케이스를 빠르게 실행(병목을 제거)</li>
  <li>병렬성을 통한 성능 고려</li>
  <li>파이프라이닝을 통한 성능 고려</li>
  <li>예측을 통한 성능 고려</li>
  <li>메모리 계층 구조</li>
  <li>중복성을 통한 신뢰도 향상</li>
</ol>

## Below Your Program

<ul>
  <li>계층구조(하위->상위): Hardware->Systems software-> Applications software</li>
  <ul>
    <li style="font-size:15px;">하드웨어와 시스템 소프트웨어 사이에 hardware/software interface존재</li>
    <li style="font-size:15px;">응용소프트웨어와 하드웨어는 직접적으로 상호작용 불가능</li>
    <li style="font-size:15px;">응용소프트웨어와 하드웨어가 상호작용하려면 시스템소프트웨어 필요</li>
  </ul>
  <li>Instruction set architecture(ISA): 
  hardware/software interface
  <li>Application binary interface(ABI): 
  The ISA + System software interface
  <ul>
    <li style="font-size:15px;">오래된 hw, 새로운 sw는 호환되지 않음(forward compatibility). 반대로, 새로운 hw, 오래된 sw는 호환가능(backward compatibility). 오래된 hw의 Instruction set의 범위가 새로운 sw를 커버할 수 없음. Instruction set은 hw가 업그레이드 될때마다 수정되는 것이 아닌, 기존의 것에 추가로 더해짐.</li>
</ul>
