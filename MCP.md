# MCP 목록

MCP는 미리 설치하지 않는다. 기본 도구로 해결하기 어렵고 사용 전제에 맞을 때만 검토한다.
새 MCP 설치 전 용도·접근 범위를 알리고 확인받는다(사용자가 직접 설치를 요청했다면 제외). 로그인 없이 쓸 수 있는 것만 둔다.

| MCP | 사용 전제 | 설명 | 공식 문서 |
| --- | --- | --- | --- |
| **Hugging Face MCP** | 공개 모델·데이터셋을 찾거나 비교해야 하는데 웹 검색으로 정확한 정보를 얻기 어려울 때 | Hub의 공개 모델·데이터셋·Spaces를 검색하고 조회한다. 로그인 없이 연결해 공개 조회 도구만 쓴다. | [설치 및 사용법](https://github.com/huggingface/hf-mcp-server) |
| **MLflow MCP** | MLflow로 실험을 기록하는 프로젝트에서 여러 실험·트레이스를 비교해야 할 때 | 로컬 MLflow의 실험과 트레이스를 조회한다. MLflow 3.5.1 이상이 필요한 실험 단계 기능이다. | [설치 및 사용법](https://mlflow.org/docs/latest/genai/mcp/) |
| **Jupyter MCP** | 노트북으로 작업하는 프로젝트에서 셀을 실행하며 결과를 확인해야 할 때 | 로컬 Jupyter 노트북의 셀을 실행하고 결과를 읽는다. | [설치 및 사용법](https://github.com/datalayer/jupyter-mcp-server) |
