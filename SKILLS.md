# Skill 목록

스킬은 미리 설치하지 않는다. 기본 AI 도구로 해결하기 어려운 작업에서만 아래 전제를 확인한다.
사용 전제를 충족해도 해당 작업에 필요한 스킬만 설치한다. 로그인 없이 쓸 수 있는 것만 둔다. 사용 동의가 필요한 모델(gated)이나 비공개 자료는 토큰이 있어야 한다.

| Skill | 사용 전제 | 설명 | 원본 |
| --- | --- | --- | --- |
| **huggingface-datasets** | 학습 전에 Hub 공개 데이터셋의 구조·내용을 내려받지 않고 확인해야 할 때 | Dataset Viewer API로 메타데이터와 행을 조회하고 검색·필터한다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-datasets) |
| **hf-mem** | 학습·추론 전에 모델이 GPU 메모리에 들어갈지 확인해야 할 때 | 가중치를 내려받지 않고 필요한 메모리를 추정한다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/hf-mem) |
| **trl-training** | TRL로 언어 모델을 파인튜닝하는데 기본 문서만으로 설정을 정하기 어려울 때 | SFT·DPO 등 TRL 학습 설정을 안내한다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/trl-training) |
| **huggingface-community-evals** | Hub 모델을 표준 벤치마크로 평가해야 할 때 | inspect-ai·lighteval로 로컬 하드웨어에서 평가한다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-community-evals) |
| **huggingface-trackio** | 프로젝트에 실험 기록 도구가 없어 학습 지표를 기록·비교해야 할 때 | Trackio로 학습 지표를 기록하고 조회한다. Space 동기화는 기본이 공개라 쓰지 않는다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-trackio) |
| **huggingface-papers** | 논문 내용이나 연결된 모델·데이터셋을 확인해야 할 때 | Hugging Face 논문 페이지를 Markdown과 메타데이터로 조회한다. | [Hugging Face](https://github.com/huggingface/skills/tree/main/skills/huggingface-papers) |

## 설치 명령

설치 전 [공식 저장소](https://github.com/huggingface/skills)의 최신 안내를 확인한다.

Claude Code에서는 저장소를 등록한 뒤 `hf` CLI로 스킬을 추가한다.

```bash
/plugin marketplace add huggingface/skills
/plugin install hf-cli@huggingface/skills
hf skills add <스킬명>
```

Codex CLI에서는 공식 저장소의 `skills/<스킬명>` 폴더를 프로젝트의 `.agents/skills/`에 복사한다.
