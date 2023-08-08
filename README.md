# Парсер документации Python
Учебный проект Яндекс Практикум (курс Python-разработчик плюс)

## Описание
Парсер документации Python имеет четыре режима работы:
1. `whats-new` - собирает ссылки на статьи о нововведениях в Python, переходит по ним и забирает информацию об авторах и редакторах статей;
2. `latest-versions` - собирает информацию о статусах версий Python;
3. `download` - скачивает архив с актуальной документацией;
4. `pep` - считает количество PEP в каждом статусе и общее количество PEP, сравнивая при этом статус на странице PEP со статусом в общем списке.

Вывод результатов реализован в трех видах на выбор:
- построчный вывод в консоль;
- вывод в консоль таблицей;
- сохранение в csv-файл.

## Технологии
[![Python](https://img.shields.io/badge/Python-3.9-3776AB?logo=python)](https://www.python.org/)
[![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup4-4.9-3776AB)](https://www.crummy.com/software/BeautifulSoup/)
[![Requests](https://img.shields.io/badge/Requests-2.27-3776AB)](https://requests.readthedocs.io/)

## Запуск проекта
Клонировать репозиторий и перейти в директорию проекта:
```bash
git clone https://github.com/bvsvrvb/praktikum-bs4-parser.git
```
```bash
cd praktikum-bs4-parser
```
Cоздать и активировать виртуальное окружение:
```bash
python -m venv venv
```
```bash
source venv/Scripts/activate
```
Установить зависимости из файла requirements.txt:
```bash
python -m pip install --upgrade pip
```
```bash
pip install -r requirements.txt
```
Ознакомиться со справкой и/или запустить проект в нужном режиме:
```bash
python main.py --help
```
и/или
```bash
python main.py [-h] [-c] [-o {pretty,file}] {whats-new, latest-versions, download, pep}
```
