# CHIP-seq-for-peter
CHIP-seq学习资料

### 流程
#### 上游分析
1. 质控 Fastqc
2. 修剪 [Trim Galore](https://github.com/FelixKrueger/TrimGalore)
3. 比对 BWA Bowtie2
4. 去除重复 Picard Samtools
5. 峰值检测 MACS2 PeakSeq
6. 峰值注释 ChIPpeakAnno  HOMER 
7. 差异结合分析（可选） DiffBind  MAnorm
8. 功能分析（可选）

 - [CHIP-seq标准流程](https://hbctraining.github.io/Intro-to-ChIPseq-flipped/schedule/links-to-lessons.html)
 - [MACS2](https://hbctraining.github.io/Intro-to-ChIPseq/lessons/05_peak_calling_macs.html)
 - [官方测试数据](https://github.com/hbctraining/Intro-to-ChIPseq/issues/63)

#### 下游分析
- [ChIPseeker:峰值注释](https://github.com/YuLab-SMU/ChIPseeker/tree/devel)
- [ChIPpeakAnno](https://github.com/jianhong/ChIPpeakAnno)
- [ChIP-seq downstream analysis: ChIPseeker](https://nbisweden.github.io/workshop-archive/workshop-ChIP-seq/2018-11-07/labs/lab-ChIPseeker.html)
- [微信：ChIP-seq数据分析代码笔记](https://mp.weixin.qq.com/s/AwHw-xGmxHbUeNttKQfoyA)
- [Basics of ChIP-seq data analysis](https://www.bioconductor.org/help/course-materials/2016/CSAMA/lab-5-chipseq/Epigenetics.html)

### 教程
- Ming Tang的学习笔记 https://github.com/crazyhottommy/ChIP-seq-analysis
- nf-core的教程 https://github.com/nf-core/chipseq
- R语言下游分析 https://www.bioconductor.org/help/course-materials/2016/CSAMA/lab-5-chipseq/Epigenetics.html

### WDL
- ENCODE的流程，带有html报告 https://github.com/ENCODE-DCC/chip-seq-pipeline2
