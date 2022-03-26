# Домашнее задание №3


Использую клеточную линию Hela-3.

## Основная часть

Google colab: https://colab.research.google.com/drive/19-7X2kON6Jzc3-jCyTf286eld4wFBh0c?usp=sharing

Таблица с используемыми гистоновыми метками:

| Гистоновая метка | Файл |
| ------- | ----------- |
| H2az | H2azAlnRep1.bam |
| H3k27ac | H3k27acAlnRep1.bam |
| H3k27me3 | H3k27me3StdAlnRep1.bam  |
| H3k36me3 | H3k36me3StdAlnRep1.bam  |
| H3k4me1 | H3k4me1StdAlnRep1.bam |
| H3k4me2 | H3k4me2StdAlnRep1.bam |
| H3k4me3 | H3k4me3StdAlnRep1.bam |
| H3k79me2 | H3k79me2StdAlnRep1.bam |
| H3k9ac | H3k9acStdAlnRep1.bam |
| H3k9me3 | H3k9me3AlnRep1.bam |

Полученные в результате рабоыт ChromHMM изображения:


<p float="left">
  <img src="/ChromHMM_Output/emissions_10.png" width="330" />
  <img src="/ChromHMM_Output/transitions_10.png" width="330" />
  <img src="/ChromHMM_Output/HeLa-S3_10_overlap.png" width="330" />
  <img src="/ChromHMM_Output/HeLa-S3_10_RefSeqTSS_neighborhood.png" width="400" />
  <img src="/ChromHMM_Output/HeLa-S3_10_RefSeqTES_neighborhood.png" width="400" />
</p>


Скриншоты из genome.browser:

<p float="left">
  <img src="/genome_browser/genome_browser_1.png" width="1000" />
  <img src="/genome_browser/genome_browser_2_0.png" width="1000" />
</p>

| State | Встречающиеся гистоновые модификации  | Остальные параметры | Название эпигенетического типа |
| ----- | ------------------------------------- |  ------------------ | ------------------------------ |
|   1   | H3k4me1StdAlnRep1.bam                 | Имеет низкий сигнал. | Transcribed |
|   2   | H3k4me1StdAlnRep1.bam, H3k4me2StdAlnRep1.bam, H3k27acStdAlnRep1.bam | Имеет хороший сигнал. | Enhancer |
|   3   | Нет                                   | Имеет средний сигнал. | Promoter |
|   4   | Все, кроме H3k27me3StdAlnRep1.bam и H3k36me3StdAlnRep1.bam | Большой процент TSS, CpG islands,TES, RefSeqExon. Имеет высокий сигнал.| Enhancer |
|   5   | H3k4me1StdAlnRep1.bam, H3k4me2StdAlnRep1.bam, H3k79me2AlnRep1.bam | Имеет высокий сигнал. | Enhancer |
|   6   | H3k79me2AlnRep1.bam                   | Большой процент RefSeqGene. Имеет низкий сигнал. | Transcribed |
|   7   | Нет                                   | Имеет низкий сигнал. | Transcribed |
|   8   | H3k36me3StdAlnRep1.bam и H3k79me2AlnRep1.bam | Большой процент TES. Имеет средний сигнал. | Promoter |
|   9   | Нет                                   | Большой процент ядерной ламины. Имеет низкий сигнал. | Transcribed |
|   10  | Нет                                   | Большой процент ядерной ламины. Имеет низкий сигнал. | Heterochromatin |

## Бонусная часть
