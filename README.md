# 3D-Mesh-Compression-Optimizer

## 📌 Project Overview

**다이나믹 메시 압축 소프트웨어 복잡도 분석 및 최적화**

본 프로젝트는 차세대 3D 콘텐츠 압축 표준인 **MPEG V-DMC(Video-based Dynamic Mesh Compression)** 소프트웨어의 복잡도를 분석하고, 부호화(Encoding) 속도를 최적화하기 위한 연구 과제입니다.

- **개발 기간**: 2024.02.15 – 2024.10.29 (약 9개월)
- **핵심 목표**: 프로파일링을 통한 병목 지점 파악 및 병렬 처리를 통한 부호화 속도 향상

## 🛠 Tech Stack

- **Language**: C++17
- **Parallel Computing**: OpenMP, std::async
- **Tools**: G++, CMake, Valgrind, WSL2 (Ubuntu)

## 🚀 Key Features & Improvements

### 1. 복잡도 분석 (Profiling)

- V-DMC 오픈 소스 코드 분석을 통해 주요 연산 단계별 실행 시간 및 메모리 사용량 측정.
- Val그라인드(Valgrind) 및 gprof 도구를 활용하여 부호화 과정 중 가장 많은 연산 시간이 소요되는 **병목 구간(Bottleneck)** 식별.

### 2. 병렬화 및 최적화 (Optimization)

- **병렬 처리 구현**: `VMCEncoder::compressVideoAtt` 함수의 반복문에 병렬화를 적용하여 연산 효율 증대.
- **예외 처리 및 동기화**: 공유 자원 접근 시 발생하는 `std::bad_alloc` 문제를 분석하고, `std::mutex`와 `std::lock_guard`를 활용한 임계 구역 설정을 통해 프로그램 안정성 확보.
- **메모리 최적화**: 중복 할당 방지 및 캐싱 기법을 통한 데이터 처리 속도 개선.

## 📊 Performance Results

| **Metric** | **Result** |
| --- | --- |
| **Encoding Speed** | **약 11% 향상** (기존 대비 속도 개선) |
| **Compression Quality** | 품질 하락 최소화 및 동기화 문제 해결 시도 |

> **Note**: 병렬 처리 시 발생할 수 있는 품질 저하 문제는 공유 자원 제어를 통해 일부 해결하였으며, 완전한 품질 복구는 향후 과제로 남겨두었습니다.
> 

## 📁 Repository Structure

```
├── encoder.cpp               # 최적화 및 병렬 처리가 적용된 핵심 소스 코드
├── 졸업프로젝트 결과보고서.docx   # 프로젝트 상세 분석 및 결과 보고서
├── 실행 설명서.pdf             # 환경 설정 및 빌드/실행 가이드
└── README.md                 # 프로젝트 개요 및 성과 요약
```

## 👥 Contributors

- **소한민**: 소프트웨어 구조 분석, 병목 지점 프로파일링 및 병렬화 알고리즘 최적화 개발
- **김범준**: 소프트웨어 구조 분석 및 최적화 방법론 구현
