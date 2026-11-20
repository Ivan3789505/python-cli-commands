## Создание проекта на FastApi

0) Установить [python](https://www.python.org/downloads/)
1) Создайте папку с проектом (название папки любое, например FastApi)
2) Откройте папку в VSCode `File` -> `Open Folder...`
3) Внутри папки создайте два файла:
    - main.py
       ```
      from fastapi import FastAPI
      
      app = FastAPI()
      
      @app.get("/")
      def read_root():
          return {"message": "Привет, FastAPI!"}
      ```
    - requirements.txt
      ```
      fastapi[standard]
      ```

4) Откройте терминал VSCode через `Ctrl + Ё` или другой терминал (например git bash или PowerShell)
5) Введите команду в терминале `python -m venv venv` (или `python3 -m venv venv`) для создания виртуального окружения
   Критерий выполнения: Должна создаться папка `venv`
6) Активация venv
    - `.\venv\Scripts\Activate.ps1` - активировать окружение в PowerShell
    - `source venv/Scripts/activate` - активировать окружение в Bash/Zsh<br>
Критерий выполнения: В терминале должно появиться `(venv)`
7) `pip install -r requirements.txt`
8) Для запуска проекта нужно ввести `fastapi dev main.py` или `uvicorn main:app --reload`
9) После успешного запуска перейти по ссылке `127.0.0.1:8000` или `localhost:8000`
