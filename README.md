# pre-commit-usage
0) `pip install pytest`, 
   `pip install pre-commit`
1) Состыковать проект с GitHub (создать новый репозиторий или взять имеющийся)
	`git init`, `git add FILES`
2) Создать файл `.pre-commit-config.yaml` (обязательное название) со всеми хуками
3) `pre-commit install`
4) `git add .pre-commit-config.yaml`
5) Проверить, что pre-commit hooks добавились в Гит командой git status. Файл .pre-commit-config.yaml должен быть в репозитории
6) `git commit -m "COMMIT_NAME"`. После выполнения этой команды должны вывестись результаты всех хуков. Если какой-либо файл в результате будет изменён, то его нужно повторно добавить в репозиторий командой `git add FILE NAME`. Повторить `git commit`
7) `git push`

## pytest-check-id

Для хука pytest-check-id необходима библиотека `pytest` и файл с назвавнием `*_test.py`, в котором лежат все желаемые функции для тестирования. Название функций также должно начинаться с `test_*`
 
