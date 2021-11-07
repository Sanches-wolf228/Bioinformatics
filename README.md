# hse21_H3F3A_ZDNA_human

Александр Крупецков БПМИ197

Гистоновая метка - H3F3A

Файлы, выбранные для анализа (human hg19, bipolar neuron)

* [ENCFF068SXT](https://www.encodeproject.org/files/ENCFF068SXT/)

* [ENCFF959PEX](https://www.encodeproject.org/files/ENCFF959PEX/)

# Анализ пиков гистоновой метки

## 1

wget https://www.encodeproject.org/files/ENCFF068SXT/@@download/ENCFF068SXT.bed.gz

wget https://www.encodeproject.org/files/ENCFF959PEX/@@download/ENCFF959PEX.bed.gz

Скачиваем данные

## 2

zcat ENCFF068SXT.bed.gz | cut -f1-5 > H3F3A_bipolar_neuron.ENCFF068SXT.hg38.bed

zcat ENCFF959PEX.bed.gz | cut -f1-5 > H3F3A_bipolar_neuron.ENCFF959PEX.hg38.bed

Распаковываем и обрезаем по 5 строчкам

## 3

http://genome.ucsc.edu/cgi-bin/hgLiftOver

На этом сайте приводим bed-файлы к нужной версии генома

Скачиваем файлы

## 4

Запускаем ноутбук build_hist.ipynb

Внутри него мы рисуем гистограммы и фильтруем файлы по длине участков.

![image](https://user-images.githubusercontent.com/71072356/140648907-e28d51cd-6b75-4456-b2bb-9bd29554577d.png)

![image](https://user-images.githubusercontent.com/71072356/140648918-742a28f5-89f6-4939-b17f-096f8ac13acb.png)

![image](https://user-images.githubusercontent.com/71072356/140648926-a83b718a-bcd6-449b-b632-421ab7855c36.png)

Мы выбрали параметры фильтрации - 4000 для ENCFF068SXT и 1500 для ENCFF959PEX

# Расположение пиков гистоновой метки относительно аннотироанных генов
