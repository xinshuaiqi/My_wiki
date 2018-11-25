s3 bucket的问题：
1) 哪些数据上传到s3: cleaned fasta reads, mapped-merged-sorted-bam, vcf?
1) de novo: contigs, scaffolds, (tgz). 
过程中产生的文件不必保存，特别是如果size大的话

2) 是否压缩上传 (或许没必要，因为压缩以后不能调用了。)： https://www.cnblogs.com/joshua317/p/6170839.html
# gzip tar 这个是性价比最高的
tar -zcvf file.tgz dir 
tar -zxvf examples.tar -C /path
# bz 压缩的更小一点儿，但费CPU，费时间多好多
tar -jcvf example.tar.bz2 examples
tar -jxvf file.tar.bz2 -C

3) 每个项目创建一个文件夹。所有的数据都放在一个文件夹里。看看有没有metadata可以注释。没有的话就建一个readme file

4) 使用Rstudio进行文件处理应该会比较快。至少比 方便很多。
5) create s3 folder with year and month, such as 201806
6) for each project, including all the readme.md, key scripts, and log files.
7) including statistics for the fasta and bam file.


More reference
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5072699/
https://onlinelibrary.wiley.com/doi/full/10.1002/humu.22368

