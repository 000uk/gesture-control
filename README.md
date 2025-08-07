# 환경설정 명령어 모음 (WSL + Python 가상환경)

```bash
# 1. WSL 실행(종료는 exit)
wsl

# 2. 프로젝트 폴더 생성 및 이동
mkdir myproject && cd myproject

# 3. 가상환경(venv) 설치
sudo apt update
sudo apt install python3.10-venv

# 4. 가상환경 생성
python3 -m venv .venv

# 5. 가상환경 활성화(나가는건 deactivate)
source .venv/bin/activate

# 6. pip 업그레이드
python3 -m pip install --upgrade pip

# 7. 필요한 패키지 설치
python3 -m pip install ultralytics
python3 -m pip install notebook

# 8. 패키지 버전 저장
pip freeze > requirements.txt

# 9. (다른 환경에서) 패키지 일괄 설치 (venv 활성화 상태)
pip install -r requirements.txt

# 10. VSCode 실행
code . (ctrl+shift+p 눌러서 Python: Select Interpreter 입력 후 venv 선택)

# 11. Jupyter Notebook 실행
jupyter notebook

