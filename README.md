### 환경설정 하는법
1. wsl(Ubuntu) 실행(나가는건 exit)
wsl

2. 프로젝트 폴더로 이동
mkdir myproject && cd myproject

3. 가상환경(venv) 설치
sudo apt update
sudo apt install python3.10-venv

4. 가상환경(venv) 생성
python3 -m venv .venv

5. 가상환경 활성화(나가는건 deactivate)
source .venv/bin/activate

6. 필요한 패키지 설치
python3 -m pip install --upgrade pip
python3 -m pip install ultralytics
python3 -m pip install notebook

7. 패키지 버전 관리용 파일(venv 활성화 상태)
pip freeze > requirements.txt
(남들은 일케 다운받음 pip install -r requirements.txt)


+ vscode 실행
code .
(ctrl+shift+p 눌러서 Python: Select Interpreter 입력 후 venv 선택)

+ Jupyter Notebook 실행
jupyter notebook


