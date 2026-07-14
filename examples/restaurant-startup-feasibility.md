# Example: Restaurant Startup Feasibility (외식업 창업 타당성 분석)

## Scenario

You are considering opening a Korean BBQ restaurant and want the skill to run a full feasibility analysis before you commit capital.

## Prompt

```text
강남역 근처에 1인 고깃집을 창업하려고 해. 보증금 5천, 권리금 8천, 인테리어 6천, 월세 350만원이야. 20평, 좌석 24석. 객단가 15,000원 예상. 타당성 분석해줘.
```

## Example Output Excerpt

```text
손익분기 분석

투자 총액: 1.9억원 (보증금 5천 + 권리금 8천 + 인테리어 6천)
별도 필요: 장비 2-3천 + 운전자금 1.5천 (3개월) = 최소 2.3억 확보 필요

월 고정비 산출:
- 월세: 350만
- 인건비 (2인 기준): 450만
- 공과금/기타: 120만
- 감가상각: 130만 (인테리어+장비 5년)
- 합계: 약 1,050만원/월

변동비: 식재료 33% 가정

손익분기 매출 = 1,050만 / (1 - 0.33) = 약 1,567만원/월
손익분기 일매출 = 1,567만 / 26일 = 약 60만원/일
손익분기 객수 = 60만 / 15,000원 = 40명/일

좌석회전율 필요: 40명 / 24석 = 1.67회전/일

판단:
- 1인 고깃집 특성상 회전율 높음 (식사 30-40분). 점심 1.5회전 + 저녁 1.0회전 = 2.5회전 가능. BEP 도달 가능성 있음.
- 그러나 권리금 8천 회수기간 = 순이익 300만 가정 시 27개월. 이는 리스크 높음.
- 임대료 비율: 350만 / 1,567만 = 22%. 위험 수준. 매출 2천만 달성 시 17.5%로 개선.

핵심 리스크:
1. 권리금 회수 27개월 — 계약기간 5년 이상 확보 필수
2. 임대료 비율 22% — BEP 수준에서는 과다
3. 1인 고깃집 경쟁 심화 — 강남 반경 500m 내 동종업종 수 확인 필요

다음 단계:
- 현장 유동인구 카운트 (점심 11:30-13:30, 저녁 17:30-20:30)
- 반경 300m 경쟁점포 조사 (같은 콘셉트 몇 개?)
- 임대차 계약서 갱신 조항 확인 (5년 보장 가능?)
```

## What Good Looks Like

The analysis should not stop at math. It should:

- calculate BEP in daily covers and required seat turnover
- assess whether the turnover rate is realistic for the concept
- flag the top 3 risks with severity
- end with concrete next steps before signing the lease
- challenge assumptions (food cost %, labor model) that the user hasn't validated

## When to Push Back

If the user's numbers don't add up (e.g., 임대료 비율 >20%, 권리금 회수 >30개월, no working capital reserved), the skill should challenge before producing the full analysis. One turn of pushback, then proceed if the user insists.
