````markdown
---

## Quick‑start: QSDsan‑tutorials (English)

### ✅ Verified

Verified on 2025‑07‑07

### 📋 Requirements

* **Anaconda** (tested with Python 3.12)
* **uv** package manager (latest)

### ⚙️ Installation Steps

```bash
# 1. Clone the repository  
git clone https://github.com/easywoo8080/QSDsan-tutorials.git
cd QSDsan-tutorials

# 2. Create Conda environment  
conda create -n qsdsan_env python=3.12 -y
conda activate qsdsan_env

# 3. Synchronize dependencies  
uv sync --dev
````

### ⚠️ Important: Pin Biosteam Version

* **TICTOC** is included only up to `Biosteam 2.51.18`.
* From `2.51.19` onward, TICTOC is removed, causing tutorials to fail.

```bash
# Roll back if upgraded  
uv add biosteam==2.51.18
uv sync
```

Add same pin to `pyproject.toml` if necessary.

### ▶️ Activate the Virtual Environment

```bash
# Conda
conda activate qsdsan_env

# venv (Windows)
.venv\Scripts\activate
```

### ▶️ Launch Jupyter Notebook

To start working with the tutorials interactively, run:

```bash
jupyter notebook
```

This will open the Jupyter Notebook interface in your browser where you can run and edit the tutorial notebooks.

---

## QSDsan‑tutorials 빠른 시작 (한국어)

### ✅ 실행확인

2025‑07‑07 실행확인

### 📋 요구 사항

* **Anaconda** (Python 3.12에서 테스트됨)
* **uv** 패키지 매니저 (최신 버전)

### ⚙️ 설치 절차

```bash
# 1. 저장소 클론  
git clone https://github.com/easywoo8080/QSDsan-tutorials.git
cd QSDsan-tutorials

# 2. Conda 환경 생성  
conda create -n qsdsan_env python=3.12 -y
conda activate qsdsan_env

# 3. 의존성 동기화  
uv sync --dev
```

### ⚠️ 중요: Biosteam 버전 고정

* **TICTOC** 모듈은 `Biosteam 2.51.18`까지만 포함됩니다.
* `2.51.19` 이상에서는 TICTOC이 제거되어 튜토리얼이 중단됩니다.

```bash
# 버전이 올라갔다면 즉시 롤백  
uv add biosteam==2.51.18
uv sync
```

필요하면 `pyproject.toml`에도 같은 버전을 명시하십시오.

### ▶️ 가상환경 실행 방법

```bash
# Conda
conda activate qsdsan_env

# venv (Windows)
.venv\Scripts\activate
```

### ▶️ 주피터 노트북 실행

튜토리얼을 인터랙티브하게 실행하려면 아래 명령어로 주피터 노트북을 시작하십시오.

```bash
jupyter notebook
```

웹 브라우저에서 노트북 인터페이스가 열리며, 여기서 튜토리얼을 실행하고 편집할 수 있습니다.

