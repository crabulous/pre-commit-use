# pre-commit-use

1) Состыковать проект с GitHub (создать новый репозиторий или взять имеющийся)
	`git init`, `git add FILES`
2) `pip install pre-commit`
3) Создать файл `.pre-commit-config.yaml` (обязательное название) со всеми хуками
4) `pre-commit install`
5) `git add .pre-commit-config.yaml`
6) Проверить, что pre-commit hooks добавились в Гит командой git status. Файл .pre-commit-config.yaml должен быть в репозитории
7) `git commit -m "COMMIT_NAME"`. После выполнения этой команды должны вывестись результаты всех хуков. Если какой-либо файл в результате будет изменён, то его нужно повторно добавить в репозиторий командой `git add FILE NAME`. Повторить `git commit`
8) `git push`

P.S.: Для хука pytest-check-id необходим файл с назвавнием `*_test.py`, в котором лежат функции от `pytest`. Название функций также должно начинаться с `test_*`
 
