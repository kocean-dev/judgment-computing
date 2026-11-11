# 판단 컴퓨팅: 핵심 개념 용어집 및 분류 체계 (Conceptual Glossary & Taxonomy)

> **Version 2.0.1** — 2026년 11월  
> **저자**: YL Khim  
> **DOI**: [10.5281/zenodo.23388471](https://doi.org/10.5281/zenodo.23388471)  
> **라이선스**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

[English Manifesto](README.md) • [한국어 선언문](README.Ko.md) • [Architecture (EN)](ARCHITECTURE.md) • [아키텍처 (KO)](ARCHITECTURE.Ko.md) • [Glossary (EN)](GLOSSARY.md) • [용어집 (KO)](GLOSSARY.Ko.md)

---

## 개요 (Overview)

본 용어집은 **판단 컴퓨팅 (Judgment Computing: AI 컴퓨팅의 마지막 질문)**에서 정립된 핵심 개념, 기본 원칙, 아키텍처 전문 용어를 정의한다. 단순한 대화형 지능을 넘어 권한(Authority), 헌법 거버넌스(Constitutional Governance), 실행 검증(Execution Verification), 그리고 인간 주권에 기반한 판단(Human-Sovereign Judgment)을 다루는 시스템을 위한 벤더 중립적 표준 분류 체계를 확립하는 것을 목적으로 한다.

---

## 핵심 분류 체계 (Core Taxonomy)

### 1. 판단 컴퓨팅 (Judgment Computing)
명령(Command), 애플리케이션(Application), 워크플로우(Workflow), 일(Work), 의도(Intent), 맥락(Context), 신뢰와 헌법(Trust & Constitutional) 컴퓨팅을 잇는 차세대 컴퓨팅 패러다임. 정당성을 가진 복수의 원칙이나 규칙이 서로 충돌하고, 정보가 불완전하며, 의사결정이 가치 우선순위 평가와 도덕적·법적 책임을 수반하는 상황을 다루는 이론적·아키텍처적 체계이다.

### 2. 판단을 인식하는 컴퓨팅 (Judgment-Aware Computing)
판단 컴퓨팅의 현실적 시스템 구현 모델. 기계가 주관적 가치를 제멋대로 계산하거나 독단적으로 시뮬레이션하는 대신, 다음과 같이 작동하도록 구조적으로 설계된 시스템을 뜻한다:
1. 결정론적 규칙 실행 영역과 가치가 걸린 판단 영역을 명확히 구분한다.
2. 규칙과 가치 간의 충돌 상황을 투명하게 식별한다.
3. 위험도를 정량화하고, 과거 판례(Precedents)를 제시하며, 대안적 선택지를 정렬한다.
4. 시스템의 경계 한계나 헌법적 임계점에 도달했을 때 스스로 멈춰 서서 인간 최종 권한(Human Final Authority)에 결정권을 양보한다.

### 3. 의도 계약 (Intent Contract)
인간 사용자와 자율 시스템 간에 상호 합의되고 암호학적으로 검증 가능한 명시적 운영 계약. 사용자의 불완전한 자연어 의도를 구속력 있는 실행 명세서로 형식화하며 다음 항목들을 포함한다:
- 허용된 작업 목표 및 명시적으로 제외된 범위(Out-of-Scope)
- 인가된 데이터 접근 범위 및 위임된 자격 증명
- 필수 검증 체크포인트(동기식 승인 게이트)
- 사전 승인된 롤백(취소) 및 보상(Compensation) 경로

### 4. 의도 탐색 (Intent Discovery)
시스템이 실행에 돌입하기 전, 사용자의 초기 발화에 내포된 모호성, 암묵적 가정, 누락된 제약 조건, 잠재적 위험을 상호작용을 통해 식별하는 초기 발견 단계. 성숙한 시스템은 **맹목적인 즉시 실행보다 탐색과 협상을 우선**한다.

### 5. 기능과 권한의 분리 (Capability vs. Authority)
다음 명제를 선언하는 근본적 아키텍처 원칙:
> *지능은 기능일 뿐, 결코 권한이 아니다 (Intelligence is capability; it is never authority).*

시스템이 특정 작업을 수행할 수 있는 연산 능력, 도구 인터페이스, API 접근 권한(기능, Capability)을 가지고 있다고 해서 행동할 수 있는 것은 아니다. 의도 계약을 통해 명시적이고 정당한 위임(권한, Authority)을 부여받지 않는 한 시스템은 결코 스스로 행동을 개시할 수 없다.

### 6. 정책보다 물리 (Physics Over Policy)
금지된 행동을 프롬프트 지침이나 사후 감사 정책으로 경고하는 대신, 환경의 경계(Boundary) 계층 수준에서 **구조적·물리적으로 불가능하게 차단**해야 한다는 보안 아키텍처 원칙. 인가되지 않은 실행 경로는 시스템 내에 통로(채널) 자체가 아예 존재하지 않아야 한다.

### 7. 경계 (Boundary / Behavior Layer)
부품(Component), 데이터, 작업 단위 간의 상호작용 방식을 규정하는 규칙 기반 행동 계층. 경계는 부품이 **무엇을 할 수 있는가(기능, Capability)**와 **어떤 조건에서 어떻게 작동하는가(행동, Behavior)**를 완벽히 분리한다.
- **UX 관점**: 부품의 논리적 연결 관계를 화면 좌표와 분리하여, 자유로운 테마 디자인과 AI 기반 인체공학적 배치를 지원한다. 평소 화면 뒤에 숨어 있다가 특정 조건에만 나타나는 부품의 유연한 결합도 포함된다.
- **보안 관점**: 허가되지 않은 접근을 원천 차단하는 뚫을 수 없는 구조적 성벽(*Physics Over Policy*)으로 기능한다.

### 8. 헌법 보존과 엔진 교체 (Preserve the Constitution, Replace the Engines)
하부 AI 모델과 실행 엔진은 급격히 발전하고 수시로 교체되지만, 시스템의 규범적 기준, 가치 우선순위, 불가침의 경계는 모델 바깥의 독립적인 **헌법 계층(Constitutional Layer)**에 영구히 보존되어야 한다는 아키텍처 격언.
- 시스템은 브라우저를 바꾸듯 AI 엔진을 자유롭게 교체한다.
- 반면 헌법은 흔들리지 않고 투명하게 감사 가능하며 온전히 보존된다.

### 9. 헌법 (Constitution / Operational Framework)
시스템 또는 조직 내의 모든 정책, 계약, 위임, 런타임 복구 전략을 지배하는 최상위 규범 체계:
> **인간 주권 (Human Sovereignty) → 가치 (Values) → 원칙 (Principles) → 헌법 (Constitution) → 거버넌스 및 정책 (Governance & Policies) → 런타임 실행 (Runtime Execution)**

- 도메인(의료, 금융, 개인 비서 등)에 따라 특화된 헌법이 존재할 수 있으나, 모든 헌법은 **인간의 최종 권한과 책임**이라는 불가침의 전제를 공유한다.
- 헌법 개정은 일상적인 정책 오버라이드와 분리되어 물리적으로 격리되고 다자간 승인이 요구되는 엄격한 절차를 거친다.

### 10. 일의 기억 (Memory of Work / Transformation Memory)
단순한 파일 스냅샷, 창 위치 복원, 혹은 대화 텍스트 기록에 머무르지 않고, **작업이 변환되어 온 궤적(Transformation Trajectory)**을 기록하는 영속성 모델:
> **원시 실행 로그 (Raw Execution Log) → 패턴 발견 (Pattern Discovery) → 작업 지식 (Work Knowledge)**

결과물이 왜 그런 형태로 만들어졌는지, 초안이 어떻게 발전했는지, 과거의 갈등과 시행착오가 어떻게 해결되었는지를 보존한다. 단순 대화 기록 대신 일의 진화 궤적을 지식으로 증류함으로써 대화 문맥의 비대화와 왜곡을 방지하고 장기적인 작업 맥락을 보존한다.

### 11. 작업 단위 (Work Unit)
애플리케이션 창(Window)을 대체하는 인간 컴퓨팅 활동의 근본 원시 단위(Primitive). 특정 인간 목적(예: *고객 장애 대응*, *세미나 준비*)을 중심으로 기능 부품, 의도, 맥락 기억, 경계 규칙을 하나로 결속한다. 작업 단위는 더 큰 작업 단위 내부에 재귀적으로 중첩될 수 있다(*Recursive Work Nesting*).

### 12. 설명 가능한 예외와 판례 (Justified Override & Precedent)
응급 상황이나 중대한 위기 상황(예: 의식불명 환자의 과거 병력을 긴급 조회해야 하는 응급실 상황)에서 권한을 가진 인간이 표준 규칙을 일시적으로 우회할 수 있도록 지원하는 구조화된 메커니즘.
- 시스템이나 헌법을 몰래 바꾸지 않는다.
- 누가 규칙을 우회했는지, 왜 정당화되었는지, 어떤 상위 가치를 구하기 위함이었는지, 어떤 위험을 감수했는지를 투명하게 기록하여 미래 감사와 검토를 위한 **판례(Precedent)**로 남긴다.

### 13. 점진적 활성화 (Progressive Activation: L0 ~ L4)
시스템 신뢰성과 성능을 위한 자원 최적화 원칙: *목적 달성에 필요한 최소한의 복잡성만 활성화한다*.
- **Level 0 (명령, Command)**: 단순 도구 및 단발성 액션 직접 호출 (열기, 인쇄, 저장).
- **Level 1 (조립, Composition)**: 작업 표면 위에서 모듈형 기능 부품의 직관적 결합.
- **Level 2 (경계 실행, Boundary Execution)**: 조건부 로직 및 데이터 흐름 규칙 실행.
- **Level 3 (지식 및 거버넌스, Knowledge & Governance)**: 의도 계약 검증, 정책 준수 확인, 승인 게이트.
- **Level 4 (형식 검증 및 복구, Verification & Recovery)**: 형식 증명 검증, 인증된 매니페스트 집행, 다계층 자율 복구.

---

## 인용 안내 (Citation)

본 용어집을 연구나 프로젝트에 인용할 경우 다음 메타데이터를 활용할 수 있습니다:

```bibtex
@misc{khim2026judgmentglossary,
  author       = {Khim, Y. L.},
  title        = {Judgment Computing: Conceptual Glossary and Taxonomy},
  year         = {2026},
  month        = nov,
  publisher    = {Zenodo},
  version      = {2.0.1},
  doi          = {10.5281/zenodo.23388471},
  url          = {https://doi.org/10.5281/zenodo.23388471}
}
```

본 저작물은 **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)** 라이선스에 따라 자유롭게 인용 및 공유될 수 있습니다.
