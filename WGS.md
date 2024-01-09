# WGS
重测序

### 分析步骤
#### 上游
- 质控 FastQC, MultiQC
- 读段修剪和过滤  Trimmomatic, Cutadapt
- 比对/序列拼接 BWA, Bowtie2 Minimap2
- 排序和标记重复 SAMtools, Picard Tools
- 变异检测  GATK, Samtools, FreeBayes, DeepVariant
- 变异过滤和注释  GATK, SnpEff, ANNOVAR
- 结构变异分析 Manta, CNVnator, BreakDancer
#### 下游分析
- 变异解释和分类：确定检测到的变异（SNVs, Indels, CNVs, SVs, MNVs等）是否与疾病相关。 ClinVar, dbSNP, 1000 Genomes Project, gnomAD, OMIM
- 基因-表型关联分析：寻找特定基因变异与表型（如疾病、性状）之间的关联。GWAS Catalog, Haploview, SNPedia
- 群体遗传学分析：研究不同人群或物种中的遗传变异。ADMIXTURE, STRUCTURE, PHYLIP
- 功能注释和通路分析：DAVID, GOrilla, KEGG PATHWAY

#### SNV
- GATK
> GATK中包含MNV
#### MNV
- [FreeBayes](https://github.com/freebayes/freebayes)
#### CNV
拷贝数变异（copy-number variant，CNV），也称拷贝数目多态性（copy-number polymorphism，CNP），是指相对于常见的二倍体基因组来说，一个大小介于 1kb 至 3MB 的 DNA 片段的变异，包括拷贝数的重复、丢失、倒位及易位，而我们所常提及的狭义的拷贝数变异指的是基因拷贝数目的改变。

![image](https://github.com/petemeng/WGS/assets/96255420/859451db-f26b-4c48-93a5-639349aea726)

- [CNVpytor](https://github.com/abyzovlab/CNVpytor/tree/master)
#### SV
- [gatk-sv](https://github.com/broadinstitute/gatk-sv)

  
### 教程
![image](https://github.com/petemeng/WGS/assets/96255420/c7c9f6d4-5ce1-4acf-87e1-4cbe44d48cdc)


- [微信：重测序教程](https://mp.weixin.qq.com/mp/appmsgalbum?action=getalbum&__biz=Mzg4NDc4MjkxNA==&scene=24&album_id=2485246989195051008&count=3&uin=&key=&devicetype=Windows+10+x64&version=63090809&lang=zh_CN&ascene=0)
- [Whole Genome Sequencing中文教程](https://github.com/flowhub-team/WholeGenomeSequencing-WGS/blob/main/README_cn.md)
- [MNV-jupyter](https://github.com/macarthur-lab/gnomad_mnv)
- [PlotCNV:An R package to create a pretty Copy Number Variant plot from a segments file](https://github.com/findlaycopley/PlotCNV)
- https://github.com/gatk-workflows/intel-gatk4-somatic-with-preprocessing
- [CNVpytor](https://github.com/abyzovlab/CNVpytor/tree/master)
- [SnpEff](https://pcingola.github.io/SnpEff/snpeff/introduction/)
- [IGV-jupyter](https://github.com/g2nb/igv-jupyter)

### Paper
- [Best practices for the interpretation and reporting of clinical whole genome sequencing](https://www.nature.com/articles/s41525-022-00295-z)


### 分析报告
- [微科盟_人类外显子重测序分析_报告（肿瘤版）](https://bioincloud.tech/cloudir/reports/WES/wes_report.html)
- [报告](https://neo-bio.cn/storage/upload/2022-10-18/1666056055_N1un.pdf)
