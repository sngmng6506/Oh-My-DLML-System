# Skill 목록

미리 설치하지 않는다. 기본 도구로 부족할 때 사용 전제에 맞는 Skill만 설치한다. 인증 없는 도구를 우선하고, 인증이 필요하면 접근 권한을 확인한다.

| Skill | 사용 전제 | 원본 |
| --- | --- | --- |
| **huggingface-datasets** | Hub 데이터셋의 메타데이터·행을 다운로드 없이 검색·확인할 때 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-datasets) |
| **hf-mem** | 모델 가중치 다운로드 없이 GPU 메모리 요구량을 추정할 때 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/hf-mem) |
| **trl-training** | 기본 문서만으로 부족한 TRL SFT·DPO 학습 설정 시 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/trl-training) |
| **huggingface-community-evals** | inspect-ai·lighteval로 로컬 표준 벤치마크 평가 시 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-community-evals) |
| **huggingface-trackio** | 기존 실험 추적 도구 없이 학습 지표를 기록·비교할 때. 공개 Space 동기화 제외 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-trackio) |
| **huggingface-papers** | 논문 Markdown·메타데이터 및 연관 모델·데이터셋 조회 시 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-papers) |
| **huggingface-best** | 공개 모델의 벤치마크 비교·후보 선정 시 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-best) |
| **huggingface-vision-trainer** | 이미지 분류·검출·세그멘테이션 학습 워크플로가 필요할 때 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-vision-trainer) |
| **train-sentence-transformers** | 임베딩·reranker 파인튜닝 시 | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/train-sentence-transformers) |

## 설치

설치 전 [공식 안내](https://github.com/huggingface/skills)를 확인한다.

Claude Code:
```bash
/plugin marketplace add huggingface/skills
/plugin install hf-cli@huggingface/skills
hf skills add <스킬명>
```

Codex CLI: 공식 저장소의 `skills/<스킬명>`을 프로젝트 `.agents/skills/`에 복사한다.
