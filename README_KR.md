<div align="center">

<div style="margin: 20px 0;">
  <img src="./assets/logo.png" width="120" height="120" alt="LightRAG Logo" style="border-radius: 20px; box-shadow: 0 8px 32px rgba(0, 217, 255, 0.3);">
</div>

# 🚀 LightRAG: 간단하고 빠른 검색 증강 생성(RAG) 프레임워크

<div align="center">
    <a href="https://trendshift.io/repositories/13043" target="_blank"><img src="https://trendshift.io/api/badge/repositories/13043" alt="HKUDS%2FLightRAG | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
</div>

<div align="center">
  <div style="width: 100%; height: 2px; margin: 20px 0; background: linear-gradient(90deg, transparent, #00d9ff, transparent);"></div>
</div>

<div align="center">
  <div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); border-radius: 15px; padding: 25px; text-align: center;">
    <p>
      <a href='https://github.com/HKUDS/LightRAG'><img src='https://img.shields.io/badge/🔥프로젝트-페이지-00d9ff?style=for-the-badge&logo=github&logoColor=white&labelColor=1a1a2e'></a>
      <a href='https://arxiv.org/abs/2410.05779'><img src='https://img.shields.io/badge/📄arXiv-2410.05779-ff6b6b?style=for-the-badge&logo=arxiv&logoColor=white&labelColor=1a1a2e'></a>
      <a href="https://github.com/HKUDS/LightRAG/stargazers"><img src='https://img.shields.io/github/stars/HKUDS/LightRAG?color=00d9ff&style=for-the-badge&logo=star&logoColor=white&labelColor=1a1a2e' /></a>
    </p>
    <p>
      <img src="https://img.shields.io/badge/🐍Python-3.10-4ecdc4?style=for-the-badge&logo=python&logoColor=white&labelColor=1a1a2e">
      <a href="https://pypi.org/project/lightrag-hku/"><img src="https://img.shields.io/pypi/v/lightrag-hku.svg?style=for-the-badge&logo=pypi&logoColor=white&labelColor=1a1a2e&color=ff6b6b"></a>
    </p>
    <p>
      <a href="https://discord.gg/yF2MmDJyGJ"><img src="https://img.shields.io/badge/💬Discord-커뮤니티-7289da?style=for-the-badge&logo=discord&logoColor=white&labelColor=1a1a2e"></a>
      <a href="https://github.com/HKUDS/LightRAG/issues/285"><img src="https://img.shields.io/badge/💬WeChat-그룹-07c160?style=for-the-badge&logo=wechat&logoColor=white&labelColor=1a1a2e"></a>
    </p>
    <p>
      <a href="README-zh.md"><img src="https://img.shields.io/badge/🇨🇳中文版-1a1a2e?style=for-the-badge"></a>
      <a href="README.md"><img src="https://img.shields.io/badge/🇺🇸English-1a1a2e?style=for-the-badge"></a>
      <a href="README_KR.md"><img src="https://img.shields.io/badge/🇰🇷한국어-1a1a2e?style=for-the-badge"></a>
    </p>
    <p>
      <a href="https://pepy.tech/projects/lightrag-hku"><img src="https://static.pepy.tech/personalized-badge/lightrag-hku?period=total&units=INTERNATIONAL_SYSTEM&left_color=BLACK&right_color=GREEN&left_text=downloads"></a>
    </p>
  </div>
</div>

</div>

<div align="center" style="margin: 30px 0;">
  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="800">
</div>

<div align="center" style="margin: 30px 0;">
    <img src="./README.assets/b2aaf634151b4706892693ffb43d9093.png" width="800" alt="LightRAG Diagram">
</div>

---

## 📖 프로젝트 개요

**LightRAG**는 지식 그래프와 벡터 검색을 결합한 차세대 검색 증강 생성(Retrieval-Augmented Generation) 시스템입니다. 전통적인 RAG 시스템의 한계를 극복하고, 문서에서 자동으로 엔티티와 관계를 추출하여 지식 그래프를 구축함으로써 더 정확하고 맥락을 고려한 답변을 생성합니다.

### 🎯 주요 특징

- **지식 그래프 기반 RAG**: 문서에서 엔티티와 관계를 자동 추출하여 구조화된 지식 그래프 생성
- **다중 검색 모드**: Local, Global, Hybrid, Mix 등 다양한 검색 전략 지원
- **15+ LLM 제공자 지원**: OpenAI, Ollama, Anthropic Claude, Google Gemini, AWS Bedrock 등
- **13+ 스토리지 백엔드**: Neo4j, MongoDB, PostgreSQL, Milvus, Qdrant 등 다양한 데이터베이스 지원
- **프로덕션 지원**: REST API, Web UI, Docker 배포 지원
- **멀티모달 지원**: RAG-Anything 통합으로 텍스트, 이미지, 표, 수식 처리 가능
- **고급 기능**: 리랭킹, 인용 추적, 문서 삭제, 평가 도구(RAGAS), 관찰성(Langfuse)

### 🏗️ 아키텍처

LightRAG는 4가지 스토리지 계층으로 구성됩니다:

1. **KV Storage**: 문서와 텍스트 청크 저장
2. **Vector Storage**: 임베딩 벡터 저장 및 유사도 검색
3. **Graph Storage**: 지식 그래프의 노드와 엣지 저장
4. **Doc Status Storage**: 문서 처리 상태 추적

---

## 🎉 최신 소식

- [2025.11] **새 기능**: RAGAS 평가 및 Langfuse 추적 통합
- [2025.10] **확장성 개선**: 대규모 데이터셋 효율적 처리 지원
- [2025.09] **새 기능**: Qwen3-30B-A3B 등 오픈소스 LLM의 지식 그래프 추출 정확도 향상
- [2025.08] **새 기능**: 리랭커(Reranker) 지원으로 혼합 쿼리 성능 대폭 향상
- [2025.08] **새 기능**: 자동 KG 재생성을 통한 문서 삭제 기능 추가
- [2025.06] **새 릴리스**: [RAG-Anything](https://github.com/HKUDS/RAG-Anything) - 올인원 멀티모달 RAG 시스템
- [2025.03] **새 기능**: 인용 기능으로 소스 추적 및 문서 출처 제공
- [2025.02] **새 기능**: MongoDB를 올인원 스토리지 솔루션으로 사용 가능
- [2025.01] **새 릴리스**: [VideoRAG](https://github.com/HKUDS/VideoRAG) - 초장편 비디오 이해를 위한 RAG
- [2025.01] **새 릴리스**: [MiniRAG](https://github.com/HKUDS/MiniRAG) - 소형 모델로 RAG를 더 간단하게
- [2024.11] **새 기능**: LightRAG WebUI - 직관적인 웹 대시보드
- [2024.11] **새 기능**: Neo4j 그래프 데이터베이스 스토리지 지원
- [2024.10] **새 기능**: Ollama 모델 지원

---

## 📦 설치 방법

> **💡 패키지 관리에 uv 사용**: 이 프로젝트는 빠르고 안정적인 Python 패키지 관리를 위해 [uv](https://docs.astral.sh/uv/)를 사용합니다.
>
> uv 설치:
> - Unix/macOS: `curl -LsSf https://astral.sh/uv/install.sh | sh`
> - Windows: `powershell -c "irm https://astral.sh/uv/install.ps1 | iex"`
>
> **참고**: pip를 사용할 수도 있지만, 더 나은 성능과 안정적인 의존성 관리를 위해 uv를 권장합니다.

### 방법 1: LightRAG Server 설치 (Web UI + API)

LightRAG Server는 Web UI와 REST API를 제공합니다. Web UI를 통해 문서 색인, 지식 그래프 탐색, 간단한 RAG 쿼리 인터페이스를 사용할 수 있습니다.

#### PyPI에서 설치

```bash
# uv 사용 (권장)
uv pip install "lightrag-hku[api]"
# 또는 pip 사용
# pip install "lightrag-hku[api]"

# 프론트엔드 빌드
cd lightrag_webui
bun install --frozen-lockfile
bun run build
cd ..

# 환경 설정 파일 생성
cp env.example .env  # .env 파일에서 LLM과 임베딩 설정을 업데이트하세요

# 서버 실행
lightrag-server
```

#### 소스에서 설치

```bash
git clone https://github.com/HKUDS/LightRAG.git
cd LightRAG

# uv 사용 (권장)
# 참고: uv sync는 자동으로 .venv/에 가상 환경을 생성합니다
uv sync --extra api
source .venv/bin/activate  # Linux/macOS
# Windows: .venv\Scripts\activate

# 또는 pip와 가상 환경 사용
# python -m venv .venv
# source .venv/bin/activate  # Windows: .venv\Scripts\activate
# pip install -e ".[api]"

# 프론트엔드 빌드
cd lightrag_webui
bun install --frozen-lockfile
bun run build
cd ..

# 환경 설정
cp env.example .env  # .env 파일 수정

# 서버 실행
lightrag-server
```

#### Docker Compose로 실행

```bash
git clone https://github.com/HKUDS/LightRAG.git
cd LightRAG
cp env.example .env  # .env 파일에서 LLM과 임베딩 설정 수정
docker compose up
```

### 방법 2: LightRAG Core만 설치 (라이브러리)

#### 소스에서 설치 (권장)

```bash
cd LightRAG
# uv sync는 자동으로 .venv/에 가상 환경을 생성합니다
uv sync
source .venv/bin/activate  # Linux/macOS
# Windows: .venv\Scripts\activate
```

#### PyPI에서 설치

```bash
uv pip install lightrag-hku
# 또는: pip install lightrag-hku
```

---

## 🚀 빠른 시작

### LLM 및 기술 스택 요구사항

LightRAG는 문서에서 엔티티-관계 추출 작업을 수행하므로 전통적인 RAG보다 LLM의 성능 요구사항이 높습니다.

- **LLM 선택**:
  - 최소 320억 파라미터 이상의 LLM 권장
  - 컨텍스트 길이는 최소 32KB, 64KB 권장
  - 문서 색인 단계에서는 추론 모델(reasoning model)을 사용하지 않는 것을 권장
  - 쿼리 단계에서는 색인 단계보다 더 강력한 모델 사용 권장

- **임베딩 모델**:
  - 고성능 임베딩 모델은 RAG에 필수적입니다
  - 다국어 임베딩 모델 권장: `BAAI/bge-m3`, `text-embedding-3-large`
  - **중요**: 임베딩 모델은 문서 색인 전에 결정해야 하며, 쿼리 단계에서도 동일한 모델을 사용해야 합니다

- **리랭커 모델 구성**:
  - 리랭커 설정으로 검색 성능을 크게 향상시킬 수 있습니다
  - 리랭커 활성화 시 "mix mode"를 기본 쿼리 모드로 설정 권장
  - 권장 모델: `BAAI/bge-reranker-v2-m3` 또는 Jina의 리랭커 서비스

### 기본 사용 예제

OpenAI API 키가 있다면 바로 데모를 실행할 수 있습니다:

```bash
# 프로젝트 폴더에서 실행
cd LightRAG

# OpenAI API 키 설정
export OPENAI_API_KEY="sk-...your_openai_key..."

# 데모 문서 다운로드 (찰스 디킨스의 "크리스마스 캐럴")
curl https://raw.githubusercontent.com/gusye1234/nano-graphrag/main/tests/mock_data.txt > ./book.txt

# 데모 코드 실행
python examples/lightrag_openai_demo.py
```

### Python 코드 예제

LightRAG를 초기화하고, 텍스트를 삽입하며, 쿼리를 수행하는 간단한 예제:

```python
import os
import asyncio
from lightrag import LightRAG, QueryParam
from lightrag.llm.openai import gpt_4o_mini_complete, gpt_4o_complete, openai_embed
from lightrag.utils import setup_logger

setup_logger("lightrag", level="INFO")

WORKING_DIR = "./rag_storage"
if not os.path.exists(WORKING_DIR):
    os.mkdir(WORKING_DIR)

async def initialize_rag():
    rag = LightRAG(
        working_dir=WORKING_DIR,
        embedding_func=openai_embed,
        llm_model_func=gpt_4o_mini_complete,
    )
    # 중요: 스토리지 초기화는 필수입니다!
    await rag.initialize_storages()
    return rag

async def main():
    try:
        # RAG 인스턴스 초기화
        rag = await initialize_rag()

        # 문서 삽입
        await rag.ainsert("여기에 텍스트를 입력하세요")

        # 하이브리드 검색 수행
        result = await rag.aquery(
            "이 이야기의 주요 주제는 무엇인가요?",
            param=QueryParam(mode="hybrid")
        )
        print(result)

    except Exception as e:
        print(f"오류 발생: {e}")
    finally:
        if rag:
            await rag.finalize_storages()

if __name__ == "__main__":
    asyncio.run(main())
```

**중요 참고사항**:
- 스크립트 실행 전에 `OPENAI_API_KEY` 환경 변수를 설정하세요
- 기본 스토리지 설정을 사용하므로 모든 데이터는 `WORKING_DIR/rag_storage`에 저장됩니다
- `await rag.initialize_storages()`는 필수 호출입니다

### Ollama 로컬 모델 사용

```python
from lightrag import LightRAG, QueryParam
from lightrag.llm.ollama import ollama_embed, ollama_model_complete

async def initialize_rag():
    rag = LightRAG(
        working_dir="./rag_storage",
        embedding_func=ollama_embed,
        llm_model_func=ollama_model_complete,
        llm_model_name="mistral",  # 또는 "qwen2.5:32b" 등
        llm_model_kwargs={"temperature": 0.7}
    )
    await rag.initialize_storages()
    return rag
```

### 프로덕션 환경: 외부 데이터베이스 사용

```python
from lightrag import LightRAG
from lightrag.llm.openai import gpt_4o_mini_complete, openai_embed

async def initialize_rag():
    rag = LightRAG(
        working_dir="./rag_storage",
        # 스토리지 백엔드 설정
        kv_storage="MongoKVStorage",
        vector_storage="MilvusVectorDBStorage",
        graph_storage="Neo4JStorage",
        doc_status_storage="MongoDocStatusStorage",
        # LLM 설정
        embedding_func=openai_embed,
        llm_model_func=gpt_4o_mini_complete,
    )
    await rag.initialize_storages()
    return rag
```

---

## 🔍 쿼리 모드

LightRAG는 다양한 검색 전략을 제공합니다:

```python
from lightrag import QueryParam

# Local 모드: 엔티티 중심, 맥락 의존적 검색
result = await rag.aquery("질문", param=QueryParam(mode="local"))

# Global 모드: 관계 중심, 전역 지식 검색
result = await rag.aquery("질문", param=QueryParam(mode="global"))

# Hybrid 모드: Local과 Global 결합
result = await rag.aquery("질문", param=QueryParam(mode="hybrid"))

# Mix 모드: 지식 그래프와 벡터 검색 통합 (기본값, 리랭커 권장)
result = await rag.aquery("질문", param=QueryParam(mode="mix"))

# Naive 모드: 기본적인 벡터 검색 (지식 그래프 미사용)
result = await rag.aquery("질문", param=QueryParam(mode="naive"))
```

### QueryParam 옵션

```python
QueryParam(
    mode="mix",                    # 검색 모드
    only_need_context=False,       # True면 컨텍스트만 반환
    only_need_prompt=False,        # True면 프롬프트만 반환
    response_type="Multiple Paragraphs",  # 응답 형식
    stream=False,                  # 스트리밍 출력 활성화
    top_k=60,                      # 검색할 상위 항목 수
    chunk_top_k=20,                # 텍스트 청크 수
    max_entity_tokens=6000,        # 엔티티 컨텍스트 최대 토큰
    max_relation_tokens=8000,      # 관계 컨텍스트 최대 토큰
    max_total_tokens=30000,        # 전체 최대 토큰
    enable_rerank=True,            # 리랭킹 활성화
    conversation_history=[],       # 대화 기록
    user_prompt=None,              # 사용자 정의 프롬프트
)
```

---

## 🎯 지원되는 LLM 제공자

LightRAG는 다양한 LLM 제공자를 지원합니다:

- **OpenAI**: GPT-4, GPT-4o, GPT-4o-mini 등
- **Ollama**: 로컬 및 클라우드 모델 (Mistral, Llama, Qwen 등)
- **Anthropic**: Claude 시리즈
- **Google Gemini**: Gemini Pro, Gemini Flash 등
- **AWS Bedrock**: Claude, Llama 등
- **Azure OpenAI**: Azure 호스팅 OpenAI 모델
- **Hugging Face**: 로컬 모델 실행
- **기타**: Zhipu, NVIDIA, LMDeploy, LlamaIndex 통합 등

자세한 LLM 설정 방법은 `examples/` 폴더의 예제를 참조하세요.

---

## 💾 스토리지 백엔드

### KV Storage (문서 및 청크)
- `JsonKVStorage` (기본값, 로컬 파일)
- `RedisKVStorage` (분산)
- `PGKVStorage` (PostgreSQL)
- `MongoKVStorage` (MongoDB)

### Vector Storage (임베딩)
- `NanoVectorDBStorage` (기본값, 경량)
- `MilvusVectorDBStorage` (분산, 확장 가능)
- `PGVectorStorage` (PostgreSQL + pgvector)
- `FaissVectorDBStorage` (Facebook AI)
- `QdrantVectorDBStorage` (벡터 데이터베이스)
- `MongoVectorDBStorage` (MongoDB)

### Graph Storage (지식 그래프)
- `NetworkXStorage` (기본값, 인메모리)
- `Neo4JStorage` (속성 그래프 데이터베이스)
- `PGGraphStorage` (PostgreSQL)
- `MongoGraphStorage` (MongoDB)
- `MemgraphStorage` (인메모리 그래프)

---

## 🛠️ 고급 기능

### 리랭킹

검색 성능을 크게 향상시키는 리랭킹 기능:

```python
from lightrag.rerank import BGEReranker

reranker = BGEReranker(model_name="BAAI/bge-reranker-v2-m3")

rag = LightRAG(
    working_dir="./rag_storage",
    embedding_func=openai_embed,
    llm_model_func=gpt_4o_mini_complete,
    rerank_func=reranker  # 리랭커 추가
)
```

### 멀티모달 문서 처리 (RAG-Anything)

PDF, 이미지, Office 문서, 표, 수식을 처리할 수 있습니다:

```python
from lightrag import LightRAG
from lightrag.modalprocessors import MultiModalProcessor

processor = MultiModalProcessor()

rag = LightRAG(
    working_dir="./rag_storage",
    embedding_func=openai_embed,
    llm_model_func=gpt_4o_mini_complete,
)

await rag.initialize_storages()

# PDF 파일 처리
await rag.ainsert_file("document.pdf", processor=processor)
```

### 평가 및 관찰성

RAGAS를 사용한 평가:

```bash
# 평가 도구와 함께 설치
uv pip install "lightrag-hku[evaluation,observability]"
```

```python
from ragas import evaluate
from lightrag.evaluation import eval_rag_quality

# RAGAS로 RAG 품질 평가
results = await eval_rag_quality(rag, test_dataset)
```

Langfuse로 LLM 호출 추적:

```python
import os
os.environ["LANGFUSE_PUBLIC_KEY"] = "your_public_key"
os.environ["LANGFUSE_SECRET_KEY"] = "your_secret_key"

# LightRAG가 자동으로 Langfuse에 추적 정보를 전송합니다
```

---

## 📚 추가 자료

- **공식 문서**: [GitHub Repository](https://github.com/HKUDS/LightRAG)
- **논문**: [arXiv:2410.05779](https://arxiv.org/abs/2410.05779)
- **튜토리얼**: [LearnOpenCV Guide](https://learnopencv.com/lightrag)
- **비디오 데모**: [YouTube](https://youtu.be/oageL-1I0GE)
- **API 문서**: [LightRAG Server README](./lightrag/api/README.md)
- **예제 코드**: [examples/](./examples/) 폴더

## 🤝 커뮤니티

- **Discord**: [LightRAG Community](https://discord.gg/yF2MmDJyGJ)
- **WeChat**: [이슈 #285](https://github.com/HKUDS/LightRAG/issues/285)
- **Issues**: [GitHub Issues](https://github.com/HKUDS/LightRAG/issues)

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다.

## 🌟 기여

기여를 환영합니다! Pull Request를 제출하거나 이슈를 열어주세요.

## 📖 인용

이 프로젝트를 연구에 사용하시는 경우 다음과 같이 인용해 주세요:

```bibtex
@article{guo2024lightrag,
  title={LightRAG: Simple and Fast Retrieval-Augmented Generation},
  author={Guo, Zirui and others},
  journal={arXiv preprint arXiv:2410.05779},
  year={2024}
}
```

---

<div align="center">
  <p>Made with ❤️ by the LightRAG Team</p>
  <p>
    <a href="README.md">English</a> •
    <a href="README-zh.md">中文</a> •
    <a href="README_KR.md">한국어</a>
  </p>
</div>
