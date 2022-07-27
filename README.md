![The Singapore Nanopore-Expression Project\!](
https://jglaborg.files.wordpress.com/2021/10/sg_nex_textlogo.png)

[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/GoekeLab/sg-nex-data?color=blue&include_prereleases)](#data-download)

The SG-NEx project is an international collaboration initiated at the [Genome Institute of Singapore](https://www.a-star.edu.sg/gis/) to provide reference transcriptomes for 5 of the most commonly used cancer cell lines using Nanopore long read RNA-Seq data:

![The Singapore Nanopore-Expression Project - Design\!](
https://jglaborg.files.wordpress.com/2020/10/sg_nex_design-1.png)

Transcriptome profiling is done using PCR-cDNA sequencing ("PCR-cDNA"), amplification-free cDNA sequencing ("direct cDNA"), direct sequencing of native RNA (“direct RNA”), and short read RNA-Seq. All samples are sequenced with at least 3 high quality replicates. For a subset of samples, we used sequin spike-in RNAs, m6A profiling using m6ACE-Seq is provided for 2 cell lines. 

The raw, aligned, and processed data is hosted on the AWS open data registry (see below for data access and analysis tutorial).


## Content

- [Email list](#sign-up-for-data-release-notifications-and-updates)
- [Latest Data Release and Access](#data-release-and-access)
- [Browse the data](#browse-the-data)
- [Data Processing](#data-processing)
- [Use Cases and Applications](#use-cases-and-applications)
- [Data Analysis Tutorials](#data-analysis-tutorials)
- [Contributors](#contributors)
- [Citing the SG-NEx project](#citing-the-sg-nex-project)
- [Contact](#contact)

## Sign up for data release notifications and updates
You can sign up for the sg-nex-updates email list to receive notifications about upcoming data releases: 

https://groups.google.com/forum/#!forum/sg-nex-updates/join

## Data Release and Access

**Latest Release (v0.3)**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5574654.svg)](https://doi.org/10.5281/zenodo.5574654)

This release includes 86 samples from 11 different cell lines. You can access the following data through the AWS Open Data Registry:

- raw files (fast5)
- basecalled files (fastq)
- aligned reads (genome and transcriptome) (bam)
- tracks for visualisation (bigwig and bigbed)
- processed data for differential RNA modification analysis (json, for use with xPore)
- processed data for identification of m6A (json, for use with m6Anet)
- annotation files
- detailed sample and experiment information

Please read the [data access tutorial](docs/AWS_data_access_tutorial.md) which describes the S3 data structure and how to access files on AWS. The direct links to the data are listed in the [sample spreadsheet](docs/samples.tsv).

_**Citation**_: Please cite the pre-print describing the SG-NEx data resource when using these data, and add the following details: "The SG-NEx data [VERSION] was accessed on [DATE] at registry.opendata.aws/sg-nex-data".

Chen, Y. _et al._ "A systematic benchmark of Nanopore long read RNA sequencing for transcript level analysis in human cell lines." _bioRxiv_ (2021). doi: https://doi.org/10.1101/2021.04.21.440736

**Release History**

You can find previous releases here in the [release history](https://github.com/GoekeLab/sg-nex-data/releases)

## Browse the data

You can now browse the data using the UCSC genome browser:

[View the SG-NEx data in the UCSC Genome Browser](http://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chrX%3A15222881%2D15533324&hgsid=1412808365_PnEkLUK7aspQOsfc7WDB6Sm93YA2)

By default only selected tracks are shown, but you can visualise all reads (bigbed tracks) and their coverage tracks (bigwig) from each individual sample.

## Data Processing

All data was aligned against the human genome version Grch38 (please refer to the [data access tutorial](docs/AWS_data_access_tutorial.md) for reference files). We collaborated with [nf-core](https://github.com/nf-core) to develop [nanoseq](https://github.com/nf-core/nanoseq), a standardardized pipeline for Nanopore RNA-Seq data processing. 

## Use Cases and Applications

You can browse a list of articles that review or use the SG-NEx data [here](/docs/SGNEx_usecases.md). If you have used the data for your own research, feel free to add a publication entry.

## Data Analysis Tutorials

The following tutorials are available that demonstrate how to analyse the SG-NEx data:

- Transcript discovery and quantification of SG-NEx samples using Bambu

- Analysing differential RNA modifications using xPore

- Identification of m6A using m6Anet

## Contributors

**GIS Sequencing Platform and Data Generation**            
Hwee Meng Low, Yao Fei, Sarah Ng, Wendy Soon, CC Khor   

**Cancer Genomics and RNA Modifications**            
Viktoriia Iakovleva, Puay Leng Lee, Lixia Xin, Hui En Vanessa Ng, Jia Min Loo, Xuewen Ong, Hui Qi Amanda Ng, Suk Yeah Polly Poon, Hoang-Dai Tran, Kok Hao Edwin Lim, Huck Hui Ng, Boon Ooi Patrick Tan, Huck-Hui Ng, N.Gopalakrishna Iyer, Wai Leong Tam, Wee Joo Chng, Leilei Chen, Ramanuj DasGupta, Yun Shen Winston Chan, Qiang Yu, Torsten Wüstefeld, Wee Siong Sho Goh

**Statistical Modeling and Data Analytics**                     
Ying Chen, Nadia M. Davidson, Harshil Patel, Yuk Kei Wan, Naruemon Pratanwanich, Christopher Hendra, Laura Watten, Chelsea Sawyer, Dominik Stanojevic, Philip Andrew Ewels, Andreas Wilm, Mile Sikic, Alexandre Thiery, Michael I. Love, Alicia Oshlak, Jonathan Göke

## Citing the SG-NEx project

If you use the SG-NEx data in your research, please specify the [release version](#data-download) and the date of access ("The SG-NEx data [VERSION] was accessed on [DATE] at registry.opendata.aws/sg-nex-data"), and cite the pre-print that describes this data resource:

Chen, Ying, et al. "A systematic benchmark of Nanopore long read RNA sequencing for transcript level analysis in human cell lines." _bioRxiv_ (2021). doi: https://doi.org/10.1101/2021.04.21.440736

## Contact

Questions about SG-NEx? Please add an entry in the [Discussions Forum](https://github.com/GoekeLab/sg-nex-data/discussions). You can also contact [Jonathan Göke](https://www.a-star.edu.sg/gis/our-people/faculty-staff)

![The Singapore Nanopore-Expression Project\!](https://jglaborg.files.wordpress.com/2020/10/sg_nex_logos-1.png)
