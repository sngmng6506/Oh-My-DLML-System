# MCP 목록

MCP는 미리 설치하지 않는다. 기본 도구로 해결하기 어렵고 사용 전제에 맞을 때만 검토한다.
새 MCP 설치 전 용도·접근 범위를 알리고 확인받는다(사용자가 직접 설치를 요청했다면 제외). 기본적으로 인증 없이 사용 가능한 도구를 우선하고, 인증이 필요하면 접근 권한을 확인한다.

| MCP | 사용 전제 | 설명 | 공식 문서 |
| --- | --- | --- | --- |
| **Hugging Face MCP** | 공개 모델·데이터셋을 찾거나 비교해야 하는데 웹 검색으로 정확한 정보를 얻기 어려울 때 | Hub의 공개 모델·데이터셋·Spaces를 검색하고 조회한다. 로그인 없이 연결해 공개 조회 도구만 쓴다. | [설치 및 사용법](https://github.com/huggingface/hf-mcp-server) |
| **MLflow MCP** | MLflow를 사용하는 프로젝트에서 실험·실행·트레이스를 조회·분석해야 할 때 | MLflow의 실험·실행·트레이스를 조회하고 분석한다. | [설치 및 사용법](https://mlflow.org/docs/latest/genai/mcp/) |
| **Jupyter MCP** | 노트북으로 작업하는 프로젝트에서 셀을 실행하며 결과를 확인해야 할 때 | 로컬 Jupyter 노트북의 셀을 실행하고 결과를 읽는다. | [설치 및 사용법](https://github.com/datalayer/jupyter-mcp-server) |
