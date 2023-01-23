POPBAM - multiregiontree
======

This fork of POPBAM fixes segmentation fault at treeData::join_tree and enables summming up multiple regions' diff matrices before calculating distance matrix for the whole tree. 

Example @RG data with required "PO"-field for merged bam file
================================================
bwa mem -t 14 -H header_sq.txt -R "@RG\tSM:SRR8177528\tID:SRR8177528.dm6.PE\tLB:0\tPL:ILLUMINA\tPU:SRR8177528_1\tPO:SRR8177528" ...

Example @SQ header for the fruit fly
====================================
@SQ	SN:chr2L	LN:23513712	AS:dm6
@SQ	SN:chr2R	LN:25286936	AS:dm6
@SQ	SN:chr3L	LN:28110227	AS:dm6
@SQ	SN:chr3R	LN:32079331	AS:dm6
@SQ	SN:chr4	LN:1348131	AS:dm6
@SQ	SN:chrM	LN:19524	AS:dm6
@SQ	SN:chrX	LN:23542271	AS:dm6
@SQ	SN:chrY	LN:3667352	AS:dm6
