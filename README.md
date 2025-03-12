### Спешл фо School21

### Использование:
#### `python3 ppcov.py [--exclude 'EXCLUDE_PATTERN']`

1. Собрать тесты с флагами `--coverage` и `-fPIC` (`gcc --coverage -fPIC some_test_files.c -o tests/build/test_runner`)
2. Прогнать тесты (`./tests/build/test_runner`)
3. Вызвать `python3 ppcov.py`
4. Чтобы убрать из репорта покрытия сами тестовые файлы, можно передать паттерн фильтрации названия файлов. Например для файлов, в названии которых есть `test_`, команда будет выглядеть так:
`python3 ppcov.py --exclude 'tests/test_*`
