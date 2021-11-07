# Bioinformatics
Homework 1

## 1

wget https://www.encodeproject.org/files/ENCFF991FFY/@@download/ENCFF991FFY.bed.gz
wget https://www.encodeproject.org/files/ENCFF863JPW/@@download/ENCFF863JPW.bed.gz

Скачиваем данные

## 2

zcat ENCFF991FFY.bed.gz | cut -f1-5 > H3K4me3_motor_neuron.ENCFF991FFY.hg38.bed
zcat ENCFF863JPW.bed.gz | cut -f1-5 > H3K4me3_motor_neuron.ENCFF863JPW.hg38.bed 

Распаковываем и обрезаем по 5 строчкам
