# medical-project

<전체적인 흐름>

데이터 분석 -> 통계 -> 배포와 같은 확장

구글 드라이브: https://drive.google.com/drive/folders/1EmSVM01WDGYz9nqjfCj1rmhh1FYdhbG0
--------------------------------------------------------------------------------------------------------------------
# 🗓 1.4
📍Today
> - 주제 정해짐
> - 보건데이터 받음 -> 연령별, 성별, 의료비용 등 통계 낼 예정.(좀 더 구체적으로 정해지면 좋을 듯) -> 확장: 헬스케어 어플, 의사 또는 병원 추천

📍내일 의논해야할 사항: 
> -  데이터 컨캣 방법 
> -  파이썬 툴로 데이터 분석이 가능할까? 파이썬 툴이 안된다면 다른 툴은 어떤 것이 있을까? ✅
> -  데이터 분석을 통하여 어떤 방식으로 통계를 낼지 
--------------------------------------------------------------------------------------------------------------------
# 🗓 1.5
📍Today: 
> - 다른 툴 사용 X, vscode나 주피터로도 충분히 가능할듯.
> - 병원, 약국 데이터 받음

📍내일 의논해야 할 사항:
> - 분석 방향 정하기
> - 병원, 약국 데이터로 매핑하는 방법 연구해보기(open api)
> - 전체 데이터 합쳐서 분석해보기 
----------------------------------------------------------------------------------------------------
----------------
# '다시 파이팅!!!!!!!!!!!!!!!!!!!!'
# 🗓 1.25
📍 오늘의 회의
> - 연령별로 주로 나타나는 질병
  : 고령화 시대와 연결 지을 수 있을까?
  : 고령화가 심화된다면 각 질병에 대한 환자수가 어떤 차이를 보일까?
  : 해외에서는 고령화 질병에 대해 어떤 대책들을 마련했을까?(일본)
  
> - 호흡기 질병 & 감기
  [가설]
    :코로나가 발생하면서 호흡기 질병 환자수는 이전보다 증가 추이를 보일 것이며, 위드코로나가 시작되면서 한번 더 증가 추이를 보일 것이다. (위드코로나: 2021년 11월, 코로나: 2020년 2월)
  [가설이 실패한 원인]
    : 연도별 추이를 보았을 때, 오히려 코로나가 시행되고 호흡기 환자수는 줄어드는 추이를 보임.
    : 마스크를 착용함으로써 호흡기 질병을 막을 수 있었고, 손씻기와 같은 청결유지를 위한 행위들을 통하여 오히려 질병이 감소한 것으로 예측(뒷받침할만한 근거-'기사')
    : 그러나! 이제 마스크 벗기 시작하면 점점 늘어날 것으로 예상. 18만정도가 줄었지만 다시 확산될 것으로 예상함(뒷받침할만한 근거-'기사')

> - 청구건수: 연도별로 변경!
> - 본인부담금
  : 난치병(혈우병,백혈병)에 대해 본인부담금이 높게 나타남
  : 난치병 환자의 완치율이 극소수이거나, 사망률이 다른 질병들과는 다르게 극명하게 높은 것으로 의견을 뒷받침 할 수 있지 않을까?
> - 치매 질병에 대해 10년 단위의 예측 데이터를 제시['확장'된 부분]
  ex) 고령화 인구가 주를 이루는 일본의 모습이 한국도 곧 겪게 될 사회적 이슈라고 판단함. 치매와 관련된 고령화 질병에 대해 일본은 어떻게 대처하고 있는지,
      한국은 이러한 이슈에 대해 어떠한 대비책을 마련해두었고, 앞으로 수정해야 할 부분은 무엇인지.
----------------------------------------------------------------------------------------------------
----------------
# 🗓 1.26
📍 오늘의 회의
- 환자에 대한 사망률, 치사율, 생존율 데이터 찾기
- 현재 보유한 질병 데이터와 연관 지을 수 있을까?
📍 각자 데이터 ppt 삽입 및 각 데이터별 피드백 제안
----------------------------------------------------------------------------------------------------
----------------
# 🗓 1.27
📍 오늘의 회의
- y축: 레이블 일정하게 맞추기(단위명+단위수)
- 시간이 지남에 따라 증가하는 질병(76위): 전체 + 남/여 + 급하게 증가하는 top10(2021-2017 환자수 값) || 고령화,저출산 + 남/여
  전체 + 남/여 + 급하게 증가하는 top10(2021-2017 환자수 값): 질병 각각에 대한 연도별 추이(라인, 바) 남,여,전체 - 나무, 질병에 대한 환자수차(바) 남,여 - 숲
----------------------------------------------------------------------------------------------------
----------------
# 🗓 1.30
📍 2017/18/19/20/21년 나이대별 발병률 높은 남/여 질병 순위
[스택] 연령분류기준으로 나눔, 전체질병(10개), 연도 5개(subplot)
- 스택 그래프 연령분류기준 나누기
  - 영유아기: ~9세
  - 청소년기: 10세 ~19세
  - 성인기: 20세 ~ 39세
  - 중장년기: 40세 ~ 59세
  - 노년기: 60세이상

[선그래프] 전연령, 남/여 각각 제외 질병 빼기(총5개), 5개년 모두 보여준 후 추후에 제거
- 남: 손상, 척추, 알레르기, (환경성질환, 치아우식증), 감기
- 여: 알레르기, 환경성질환, 영상단말기 증후군, 손상, 감기
