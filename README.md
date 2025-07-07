````markdown
## Quick‑start: QSDsan‑tutorials

2025-07-07 실행확인.

### 요구 사항
- **Anaconda**(Python 3.12 기준)  
- **uv** 패키지 매니저(최신판)

### 설치 절차
```bash
# 1. 저장소 클론
git clone https://github.com/<USER>/QSDsan-tutorials.git
cd QSDsan-tutorials

# 2. Conda 환경
conda create -n qsdsan_env python=3.12 -y
conda activate qsdsan_env

# 3. 의존성 동기화
uv sync
````

### 중요: Biosteam 버전 고정

* `Biosteam 2.51.18`까지만 **TICTOC** 모듈을 포함합니다.
* `2.51.19` 이상에서는 TICTOC이 제거되어 튜토리얼 실행이 중단됩니다.

```bash
# 버전이 올라갔다면 즉시 롤백
uv add biosteam==2.51.18
uv sync
```

필요 시 `pyproject.toml`에도 같은 버전을 명시해 두십시오.


가상환경 실행 방법
```bash
#아나콘다 가상환경
conda activate qsdsan_env

# 가상환경
.venv\Scripts\activate
```