# ⚔️ [Core Protocol] Byeorim (벼림) Grammar v1.0

**The Morphological Language for Absolute AI Orchestration**

> **[System Context: 생태계 제0 헌법]**
> 본 문서는 자율형 AI 코딩 에이전트 생태계의 3대 축(`Hwatotbul`, `Denavy`, `Registry`)이 상호 소통하고 문맥을 압축하기 위해 공유하는 **단 하나의 공용 기호 논리학 헌법**이다.
> 목적에 따라 `.hwb`, `.dna`, `.spec` 내부에 벼림 문법이 기본 탑재되며, 순수 통신 및 데이터 파일의 확장자는 `.br`을 사용한다.

## 0. 벼림(Byeorim)의 철학과 절대 원칙

**'벼리다 (To Forge & Sharpen)'**: 쇳덩이를 불에 달구어 두드림으로써 불순물을 제거하고 무딘 날을 극도로 날카롭고 옹골차게 단련하는 공학적 과정.

1. **오컴의 쳐내기 (Zero Syntactic Noise):** JSON, YAML의 괄호(`{}`), 따옴표(`""`), 쉼표(`,`)는 에이전트의 지능을 분산시키는 불순물이다. 이를 전면 불법화하며 오직 **들여쓰기(Indentation)**로만 계층을 벼려낸다.
2. **밀도의 극대화 (Symbolic Density):** 장황한 자연어 지시를 배제하고, 시각적인 '기호 룬(Rune)'만으로 제어 흐름과 상태를 100% 강제하여 AI의 환각(Hallucination) 틈새를 원천 밀봉한다.
3. **자연어의 격하 (Human Whisper):** 언어 모델을 위한 자연어 지시는 오직 인간을 위한 주석(`#`)의 형태로만 허용되며, 시스템의 논리 흐름(Control Flow)에 절대 개입할 수 없다.

---

## 1. 벼림 기호 룬 (The Runes of Byeorim)

시스템의 모든 문맥과 설계는 아래의 기호로 압축된다. 에이전트는 이 기호가 그리는 형태(Morphology) 자체를 런타임 절대 법칙으로 인식해야 한다.

### 🌐 1.1. 전역 식별 기호 (Global Anchors)

* `$ ` : **Global Symbol (단조된 식별자).** 전역 변수, 엔티티, 또는 거대한 에러 로그 덩어리를 단일 기호로 압축하여 어텐션 분산을 막는다. *(예: `$User.login`, `$ERR_DB_TIMEOUT`)*
* `# ` : **Human Whisper (인간의 속삭임).** 에이전트 실행 로직에 영향을 주지 않는 인간 전용 주석.

### 🔥 1.2. 거시적 통제 기호 (Hwatotbul Domain)

시간의 흐름, 비동기 칸반 현황, 프로젝트의 거시적 룰을 제어한다. **파이썬 런타임과 AI 오케스트레이터가 주로 스캔하고 치환하며, 워커 에이전트는 수정 권한이 없다.**

* `[ ] / [-] / [?] / [x] / [!]` : **프랙탈 칸반 상태 머신.** 파이썬 런타임에 의한 인플레이스 락(Lock) 및 워크플로우 제어. *(대기 / 락&실행중 / 결재대기 / 완료 / 모순·중단)*
* `◈ ` : **Epoch (시공간 표식).** 현재 진행 중인 마일스톤 타임스탬프.
* `⊘ ` : **Trauma (트라우마).** 절대 어겨선 안 되는 프로젝트 단위의 흉터. 환각 0순위 차단 닻.
* `∿ ` : **Dirty Ending (더티 엔딩).** 의도된 기술 부채. 기존 코드의 결함을 보고 멋대로 리팩토링하려는 에이전트의 오지랖(Vibe Coding)을 차단하는 면죄부.
* `∞ ` : **Memory.** 외부 Registry나 불변의 진리로 향하는 참조 포인터.

### 🏛️ 1.3. 미시적 실행 기호 (Denavy Domain)

워커 에이전트가 격리된 샌드박스 방에서 비즈니스 로직(`/spec`)을 기안(Draft)하고 코드(`/src`)를 구현할 때 사용하는 **절대 제어 흐름(Control Flow) 헌법**이다.

* `@ ` : **의존성 참조 (Import / Dependency).** 외부 모듈이나 데코레이터 주입.
* `! ` : **필수 제약 (Required / Immutable Guard).** 데이터 무결성 및 정책 강제. 위반 시 런타임은 즉시 샌드박스를 폭파(Halt)한다.
* `<: ` : **상속 및 확장 (Inheritance).** 선언된 뼈대를 물려받음.
* `? ` : **조건 검증 (Decision Gate).** 논리가 갈라지는 결정적 관문.
* `!=>! ` : **비명 및 조기 종료 (Absolute Halt).** 로직 모순이나 에러 발생 시 에이전트가 내지르는 단말마. 즉시 실행을 멈추고 파이썬 런타임에 제어권을 넘긴다. (에이전트 자의적 상태 수정 불가)
* `<- ` : **상태 할당 및 변환 (Mutation).** 우항의 연산 결과를 좌항에 바인딩.
* `> ` : **외부 함수/액션 실행 (Execute).** DB I/O 등 부수 효과(Side-effect)가 발생하는 행위 트리거.
* `=> ` : **정상 반환 (Success).** 해당 논리 블록의 성공적 완료 신호.

---

## 2. 벼림(Byeorim) 문법 작성 예시

아래는 벼림 문법으로 압축된 Denavy의 비즈니스 로직(Spec) 기안 예시다. 장황한 괄호와 자연어가 싹 다 벼려진(깎여나간) 초고밀도의 칼날을 확인하라.

```text
@ import: $Security.User

$User.login(credentials):
  > sanitizers.clean_input(credentials.email)
  
  ?! credentials.email.isValidFormat:
    !=>! Error("INVALID_FORMAT")

  > $User.findByEmail(credentials.email) <- user_record
  
  ! user_record.status == 'ACTIVE':  # 정책 강제. 위반 시 샌드박스 폭파
    > security.trigger_alert("Inactive user")
    !=>! Error("LOCKED")
    
  => auth.generateToken(user_record)

```

---