개념	           |  카테고리/역할	                       |                 튜터님 지식과의 연결고리	


LangChain (랭체인)	|프레임워크(Framework)	                 |       파이썬 라이브러리 및 개발 환경. Flask/Django 같은 웹 프레임워크처럼, LLM 애플리케이션 개발을 구조화.
NLP (자연어 처리)	|기술 영역 (Technology Field)	         |       전체 과정의 기본 원리. 텍스트 토큰화, 단어 임베딩, 시퀀스 투 시퀀스 학습 등 튜터님이 배우신 텍스트를 위한 딥러닝 모든 기법을 포함	
RAG (검색 증강 생성)|	애플리케이션 패턴/기법 (Pattern/Methodology)|	LLM의 성능을 향상시키는 특정 방법. 튜터님이 배우신 데이터 처리 및 데이터 생성/조작 개념

1. NLP (Natural Language Processing)역할: NLP는 LangChain과 RAG를 포함하는 모든 텍스트 기반 기술의 근본.
설명: 랭체인이나 RAG를 사용한다는 것은 기본적으로 자연어(사람의 언어)를 처리하고 이해하는 NLP의 영역 안에 있는 것
예시: 랭체인에서 사용하는 LLM 자체가 딥러닝(트랜스포머 아키텍처) 기반의 가장 발전된 NLP 모델

2. RAG (Retrieval-Augmented Generation)역할: LLM의 답변 품질과 정확성을 높이기 위한 구체적인 설계 패턴.
설명: RAG는 외부 데이터베이스나 문서를 검색(Retrieval)하여 얻은 사실 기반의 근거를 바탕으로 LLM이 생성(Generation)하도록 도움.
LangChain과의 관계: RAG를 구현할 때 LangChain을 사용하면 매우 편리.
Chain: 검색 모듈 (문서를 가져옴) rightarrow LLM 모듈 (검색된 문서를 참고해 답변 생성)의 흐름(Chain)을 쉽게 만듦.
Components: 문서 로드(Document Loaders), 분할(Text Splitters), 벡터화 및 검색(Vector Stores & Retrievers) 등 RAG의 핵심 요소를 LangChain이 제공.

3. LangChain (랭체인)역할: NLP 기술 (LLM)과 RAG 패턴을 하나의 애플리케이션으로 엮어주는 접착제(Glue)이자 인프라.
설명: 파이썬 라이브러리로 처럼, LangChain은 RAG를 포함한 다양한 복잡한 LLM 워크플로우를 파이썬 코드로 쉽게 구현할 수 있게 해줌.
