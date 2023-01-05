# medical-project

# 데이터 설명
[자료 상세설명]
○ 질병 기준: 주상병(환자의 요구가 가장 컸던 상병)
* 최종 질병과는 차이가 존재할 수 있음

○ 법정감염병: 의료기관에서 질병자에 대해 검사, 처치, 의약품처방 등 치료를 위한 진료내역을 바탕으로 산출
* 병관리본부의 법정감염병 통계자료와는 대상범위, 기준 등 차이가 존재할 수 있음

○ 식중독: 의료기관에서 질병자에 대해 검사, 처치, 의약품처방 등 치료를 위한 진료내역을 바탕으로 산출
* 식약처의 통계자료와는 대상범위, 기준등 차이가 존재할 수 있음

○ 요양급여비용총액: 요양기관 내 건강보험 환자의 진료에 소요된 비용(비급여제외) + 보험자부담금(국민건강보험공단)과 본인부담금

○ 환자수: 범주 내 동일인의 중복을 제거
* 다른 범주와 단순합산할 경우 중복이 발생할 수 있음
* 동일 수진자가 입원/외래 유형을 달리하여 진료를 받은 경우 중복 집계될 수 있음

[자료 생성규칙]
○ 건강보험(약국 직접 조제 및 처방 조제 제외, 양방만 포함)
※ [한방]~의 경우, 건강보험(약국 직접 조제 및 처방 조제 제외, 한방 상병만 포함)


<전체적인 흐름>

데이터 분석 -> 통계 -> 배포와 같은 확장

# 1.4
📍주제 정해짐
> - 보건데이터 받음 -> 연령별, 성별, 의료비용 등 통계 낼 예정.(좀 더 구체적으로 정해지면 좋을 듯) -> 확장: 헬스케어 어플, 의사 또는 병원 추천

📍내일 의논해야할 사항: 
> -  데이터 컨캣 방법
> -  파이썬 툴로 데이터 분석이 가능할까? 파이썬 툴이 안된다면 다른 툴은 어떤 것이 있을까? 
> -  데이터 분석을 통하여 어떤 방식으로 통계를 낼지.

