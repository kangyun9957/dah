# DAH 2026 — Defense AI Cyber Security Hackathon

국내 최초 방산 AI 공방전 해커톤 **DAH 2026** 출전 자료 저장소.

- 대회 공식: https://dah.ai.kr
- 주최·주관: LIG D&A (구 LIG넥스원)
- 본선: 2026.08.21 (금) · SKY31 CONVENTION (송파) · Offline
- 접수 마감: 2026.06.14
- 예선 보고서 마감: 2026.07.10

## 구성

```
preliminary-report/
  DAH2026_Defense_AI_Report.pdf   예선 제출용 보고서 (PDF, A4)
  report.html                     보고서 원본 HTML (수정 후 재변환 가능)
```

## 예선 보고서 개요

`UAV/UGV 공격 시나리오 대응 방어 AI 시스템 설계`

| 섹션 | 매핑 배점 |
|---|---|
| 3장 — 공격 시나리오 10건 (GNSS 스푸핑, MAVLink AiTM, 펌웨어/ML Trojan, 적대적 센서, SATCOM MITM, 정책망 회피, 1553B Rogue BC, 스웜 합의, 사이드채널, 자해유도 DoS) | 30pt |
| 4장 — Defense-in-Depth × Zero Trust × Resilient Control | 25pt |
| 5장 — 다중 AI 에이전트 (Sentinel · Hunter · Healer · Coordinator), LLM + RL 하이브리드 | 25pt |
| 8장 — 팀 역량 (템플릿, 제출 전 실명 교체 필요) | 10pt |
| 문서 완성도 (자동 평가) | 10pt |

## 보고서 재생성

HTML 수정 후 다음 명령으로 PDF를 다시 만듭니다 (Windows).

```powershell
& "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" `
  --headless --disable-gpu --no-pdf-header-footer `
  --print-to-pdf="preliminary-report\DAH2026_Defense_AI_Report.pdf" `
  "file:///$PWD/preliminary-report/report.html"
```

## 참고 표준 (보고서 부록 A 발췌)

- MITRE ATT&CK for ICS · ATLAS · D3FEND
- NIST SP 800-82r3 / 800-207 / 800-160 Vol.2 / IR 8270 / AI RMF 1.0
- NATO STANAG 4586 / 4609 / 4671 · MIL-STD-1553B · MIL-HDBK-1785
- MAVLink 2.0 · OMG DDS-Security v1.1 · SAE J1939
- KISA 드론 정보보호 가이드 · ENISA Drones Cybersecurity · CISA UAS 가이드

## 라이선스 / NDA

본 자료는 DAH 2026 예선 제출 목적이며, 본선 진출 시 정식 NDA 서명에 따라 공개 범위가 조정됩니다.
