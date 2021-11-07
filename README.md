# Bioinformatics
Homework 1

## 1

wget https://www.encodeproject.org/files/ENCFF068SXT/@@download/ENCFF068SXT.bed.gz

wget https://www.encodeproject.org/files/ENCFF959PEX/@@download/ENCFF959PEX.bed.gz

Скачиваем данные

## 2

zcat ENCFF068SXT.bed.gz | cut -f1-5 > H3F3A_bipolar_neuron.ENCFF068SXT.hg38.bed

zcat ENCFF959PEX.bed.gz | cut -f1-5 > H3F3A_bipolar_neuron.ENCFF959PEX.hg38.bed

Распаковываем и обрезаем по 5 строчкам
