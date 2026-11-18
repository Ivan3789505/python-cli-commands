## Создание проекта на Selenium

0) Установить [python](https://www.python.org/downloads/)
1) Создайте папку с проектом (название папки любое, например Selenium)
2) Откройте папку в VSCode `File` -> `Open File...` или сочетанием клавиш `Ctrl + O`
3) Внутри папки создайте два файла:
    - main.py (пустой)
    - requirements.txt
      ```
      selenium==4.*
      ```
4) Откройте терминал VSCode через `Ctrl + Ё` или другой терминал (например git bash или PowerShell)
5) Введите команду в терминале `python -m venv venv` для создания виртуального окружения
   Критерий выполнения: Должна создаться папка `venv`
6) Активация venv
    - `.\venv\Scripts\Activate.ps1` - активировать окружение в PowerShell
    - `venv/Scripts/activate` - активировать окружение в Bash
    Критерий выполнения: В терминале должно появиться `(venv)`
7) `pip install -r requirements.txt`
8) Для запуска скрипта нужно ввести `python main.py`
