## Quick‑start: QSDsan‑tutorials

**EN / KO**

### Verified on 2025‑07‑07 / 2025‑07‑07 실행확인

### Requirements / 요구 사항

* **Anaconda** (tested with Python 3.12)
* **uv** package manager (latest)

### Installation Steps / 설치 절차

```bash
# 1. Clone the repository / 저장소 클론
git clone https://github.com/easywoo8080/QSDsan-tutorials.git
cd QSDsan-tutorials

# 2. Create Conda env / Conda 환경
conda create -n qsdsan_env python=3.12 -y
conda activate qsdsan_env

# 3. Synchronize dependencies / 의존성 동기화
uv sync
```

### Important: Pin Biosteam Version / 중요: Biosteam 버전 고정

* **TICTOC** is included only up to `Biosteam 2.51.18`.
  **TICTOC** 모듈은 `Biosteam 2.51.18`까지만 포함됩니다.
* From `2.51.19` onward TICTOC is removed, causing tutorials to fail.
  `2.51.19` 이상에서는 TICTOC이 제거되어 튜토리얼이 중단됩니다.

```bash
# Roll back if upgraded / 버전이 올라갔다면 즉시 롤백
uv add biosteam==2.51.18
uv sync
```

Add same pin to `pyproject.toml` if necessary.
필요하면 `pyproject.toml`에도 같은 버전을 명시하십시오.

### Activate the Virtual Environment / 가상환경 실행 방법

```bash
# Conda
conda activate qsdsan_env

# venv (Windows)
```bash
.venv\Scripts\activate
```
