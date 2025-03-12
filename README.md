### Спешл фо School21
#### Замена `gcovr` / `lcov` на школьных маках

### Использование:
#### `python3 ppcov.py [--exclude 'EXCLUDE_PATTERN']`

1. Скачать `ppcov.py`
2. Собрать тесты с флагами `--coverage` и `-fPIC` </br>
(`gcc --coverage -fPIC some_test_files.c -o tests/build/test_runner`) </br>
3. Прогнать тесты </br>
(`./tests/build/test_runner`) </br>
4. Вызвать `python3 ppcov.py` </br>
5. Чтобы убрать из репорта покрытия сами тестовые файлы, можно передать паттерн фильтрации названия файлов. Например для файлов, которые лежат в папке `tests` и в названии которых есть `test_`, команда будет выглядеть так:
`python3 ppcov.py --exclude 'tests/test_*`
