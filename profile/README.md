# GlassCard – 의미 기반 단어 암기 서비스 ✨
![Home1](https://github.com/user-attachments/assets/175e1127-31ac-479c-bb54-a6a4de6390ad)

**GlassCard**는 단순 암기를 넘어서, 의미를 이해하며 단어를 학습할 수 있도록 돕는 유연한 암기 플랫폼입니다.  
정확히 일치하지 않더라도 **의미가 유사한 답변**이라면 정답으로 인정되며, 이를 통해 학습자는 보다 자연스럽게 어휘력을 키울 수 있습니다.

---

## 핵심 개념
 
- 사용자는 단어장에 등록된 단어의 뜻을 자유롭게 입력합니다.
- 입력한 답이 단어장 제작자가 설정한 정답과 **의미상 유사**하다면 정답으로 처리됩니다.
- **AI 의미 판별 모델**을 활용하여 유사도를 분석합니다.
- 단순 암기를 넘어 **이해 기반의 어휘 습득**을 유도합니다.
- 로그인 없이 바로 사용 가능하며, 학습 기록은 브라우저에 저장됩니다.


## 정답 유형 및 판별 기준

| 구분       | 설명                                      | 정답 인정 여부 |
|------------|-------------------------------------------|----------------|
| `Correct`  | 원래 단어장에 등록된 정확한 정답          | ✅              |
| `Flexible` | 의미상 유사하거나 동의어로 판단 가능한 표현 | ✅              |
| `Incorrect`| 전혀 다른 뜻                              | ❌              |

- `Correct`, `Flexible`는 모두 정답으로 인정됩니다.
- `Incorrect`는 정답으로 인정되지 않습니다.
<table width="100%">
  <tr>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/b1b4068d-395a-4d63-8c14-4d8491b0a921" width="90%" /><br/>
      <strong>Correct</strong>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/9103695e-2e0e-468e-9132-838f9277e3c4" width="90%" /><br/>
      <strong>Flexible</strong>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/9b0ab61e-808e-4cf4-9377-495c06336f4b" width="90%" /><br/>
      <strong>Incorrect</strong>
    </td>
  </tr>
</table>


## 정답 판정 방식

- 입력이 **Exact match** 또는 **Semantic match**일 경우 정답 처리
- `Flexible` 수준의 입력은 AI 기반 의미 분석을 통해 유사성 판별
- 예시: `buy`의 정답이 `purchase`인 경우 → `get`, `acquire` 등도 정답 처리 가능


## 사용 방식

- 학습 방식:  
  - 단어 → 뜻 입력  
  - 뜻 → 단어 입력
  - 예문 빈칸 → 빈칸에 들어갈 단어 입력

- 입력 유연성:  
  - 대소문자, 띄어쓰기, 복수형 등의 차이는 자동 보정됩니다.

- 학습 중 제공 기능:  
  - 정답 기준 확인
  - 유사어 목록 확인 
  - 예문 제공
  - 오답 시 유사도 피드백


## 유저 Auth

- 회원가입 없이 즉시 사용 가능
- 학습 기록은 브라우저에 자동 저장
- 단어장 생성 시 수정 password 설정 가능 -> 수정할 때 해당 password를 입력해야만 수정 가능


## 기술적 개요

- 의미 유사도 판별 모델: **s-BERT 기반 임베딩 모델**
- AI 추론 로직: 문장 단위 의미 비교, cosine similarity 기반 정답 처리


## 향후 계획

- 사용자별 단어장 클라우드 저장 기능
- 다양한 언어(예: 일본어, 스페인어 등) 지원
- 예문 자동 생성 기능
- 학습 분석 기반 개인화 추천 시스템 도입


## 팀원 소개
|[류승찬](https://github.com/winshine0326)|[조하민](https://github.com/yuuki08noah)|
|:---:|:---:|
|프론트엔드 & 디자인|프론트엔드 & 백엔드|
|<img src="https://github.com/user-attachments/assets/4d636456-d599-42da-83bb-8b0adb86cddb" width="300px" />|<img src="https://github.com/user-attachments/assets/db4117b4-930d-4b80-a58d-8393fe84734a" width="300px" />|





