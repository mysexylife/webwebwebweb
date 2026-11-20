# M4 / A4 규제·법적 리스크 검토 (regulation-feasibility 보고 요약)
검색 11회 중 9회 성공(스템 분리 소송·DDEX AI 필드 실패). suno.com 원문 차단 → Suno 약관은 2차 출처 기반(확인 불가/추정). 법률 자문 아님.
## 쟁점
- 한국: 사람 기여 부분만 등록 가능(저작권위원회 안내서 2025-06), 문체부 등록 시 AI 활용 범위 명세 의무화 추진(2026-11-12 보도) https://zdnet.co.kr/view/?no=20261112160345 ; 음저협 AI 곡 기준 8/3 시행→22일 만에 철회(사유·기존 신고 처리 확인 불가) https://view.asiae.co.kr/article/2026083116360854659
- 미국: 프롬프트만으론 저작자성 불인정 https://copyright.gov/newsnet/2025/1060.html
- 소송·합의: UMG–Udio 합의(2025-10)·다운로드 중단, WMG–Suno 합의(2025-11), UMG의 DistroKid 제소(2026-09-15, 1,000곡, 핵심은 AI 곡 위장) https://www.digitalmusicnews.com/2026/09/15/universal-music-distrokid-lawsuit/ → AI 표기(disclosure)를 하는 쪽에 유리한 환경
- Suno 약관(2차 출처): 유료만 상업 이용, 스크래핑·데이터 마이닝 금지, 경쟁 모델 개발 금지, 공식 공개 API 없는 것으로 보임 → 자동 연동은 약관 위반 가능성 높음 https://conductatlas.com/platform/suno/suno-terms-of-service/prohibition-on-data-mining-and-scraping/
- 유통: TuneCore·Believe는 비라이선스 모델 산출물 거부, 라이선스 모델(ElevenLabs, Udio, Flow Music)은 허용 https://www.musicbusinessworldwide.com/believe-and-tunecore-blocking-suno-elevenlabs-and-udio/
- 스템 분리 서비스 소송 사례는 확인 불가. 타인 곡 업로드 방조 책임 가능성(추정 Mid), 자기 생성곡만 처리하면 위험 낮음.
- 증빙 SaaS는 법적 효력 없음(등록·권리 판단은 협회·저작권위원회·법원). '법적 보호 보장' 표현은 허위·과장 광고 소지, 자기신고 로그는 위조 용이.
## 리스크 등급
- M4: 음저협 기준 철회로 수요·포맷 불확실 High / 증빙 효력 과장 책임 High / DDEX 표준 상태 확인 불가 Mid / 플랫폼 수용 의존 Mid / Critical 없음
- A4: Suno/Udio 입력 자동 수집 = **Critical(수집 자동화 시)**, 사용자 직접 업로드면 High / 출력물 유통 거부 High / Udio 다운로드 중단·Suno 한도로 원료·단가 불안정 High / 방조·복제 Mid
## 점수(에이전트는 '높을수록 위험' 척도로 기재 — criteria.md는 낮을수록 고득점이므로 변환 필요)
- M4 위험 3.0/5 (→ criteria 득점 2/5), 실행 난이도 6/10 / A4 위험 4.0/5 (→ 득점 1/5), 실행 난이도 6/10
## 사전 조치 3가지: ① Suno/Udio 약관 원문 직접 확인·공식 API/파트너십 서면 문의(확답 전 자동 수집 구조 금지, 사용자 직접 업로드 설계) ② 증빙 문구는 '참고용 기록'으로, 책임 제한 조항 변호사 검토 ③ 음저협·저작권위원회·TuneCore/Believe에 출력 포맷 수용 여부 선확인
