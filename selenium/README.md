## Создание проекта на Selenium

0) Установить [python](https://www.python.org/downloads/)
1) Создайте папку с проектом (название папки любое, например Selenium)
2) Откройте папку в VSCode `File` -> `Open Folder...`
3) Внутри папки создайте два файла:
    - main.py (пустой)
    - requirements.txt
      ```
      selenium==4.*
      ```
4) Откройте терминал VSCode через `Ctrl + Ё` или другой терминал (например git bash или PowerShell)
5) Введите команду в терминале `python -m venv venv` (или `python3 -m venv venv` для Mac) для создания виртуального окружения<br>
Критерий выполнения: Должна создаться папка `venv`
7) Активация venv
    - `.\venv\Scripts\Activate.ps1` - активировать окружение в **PowerShell**
    - `source venv/Scripts/activate` - активировать окружение в **Bash/Zsh**<br>
Критерий выполнения: В терминале должно появиться `(venv)`
8) `pip install -r requirements.txt`
9) Для запуска скрипта нужно ввести `python main.py`
