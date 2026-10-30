# 실험 기록 예시

실험마다 한 항목씩 추가하는 형식의 예시다. 아래 값은 실제 실험에 맞게 바꾼다.

## 2026-01-15 baseline-resnet18

| 항목 | 값 |
| --- | --- |
| 목적 | 베이스라인 모델 성능 확인 |
| 코드 커밋 | `a1b2c3d` |
| 데이터 | `dataset-v2` (train 8,000 / val 1,000 / test 1,000) |
| 환경 | Python 3.11, PyTorch 2.4, GPU 1장 |
| 시드 | 0, 1, 2 |
| 하이퍼파라미터 | lr 1e-3, batch 64, epoch 30 |
| 결과 (val accuracy) | 0.842 ± 0.006 (3회 평균 ± 표준편차) |
| 결과 파일 | `runs/baseline-resnet18/metrics.json` |
| 결론 | 이후 실험의 비교 기준으로 사용 |
| 실패·특이 사항 | 시드 2에서 epoch 12 이후 손실 발산, lr 낮춰 재실행 |
