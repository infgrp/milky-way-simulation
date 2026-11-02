# Milky Way Simulation

Three.js로 만든 나선은하 시뮬레이션입니다. 암흑물질 유무에 따른 은하 회전(케플러 회전 vs 평탄 회전)과, 밀도파 이론으로 나선팔이 유지되는 원리를 보여 줍니다.

**바로 보기:** https://infgrp.github.io/milky-way-simulation/

| 버전 | 내용 |
|---|---|
| [Classic](classic.html) | 별 12만 개, 밀도파로 팔의 밝기가 바뀜 |
| [Grand](grand.html) | 별 40만 개(최대 100만), 로그나선 팔, 궤도 밀집, 성운, 먼지대, 은하핵 광채 |

## 조작
- 마우스 드래그: 회전 / 휠: 확대·축소 / 우클릭 드래그: 이동
- 오른쪽 위 패널
  - **Dark Matter Factor**: 0이면 케플러 회전(바깥이 느림), 1이면 평탄 회전(암흑물질)
  - **Spiral Arms**: 팔 개수, 피치각, 밀도, 선명도 등

## 로컬 실행
ES 모듈을 쓰기 때문에 파일을 직접 열지 말고 웹 서버로 실행하세요.

```bash
python3 -m http.server 8000
# 브라우저에서 http://localhost:8000
```

인터넷 연결이 필요합니다(three.js, lil-gui를 CDN에서 불러옴).
