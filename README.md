# Galaxy

## Introduction
Galaxy is a scientific workflow, data integration, and data and analysis persistence and publishing platform that aims to make computational biology accessible to research scientists that do not have computer programming or systems administration experience. Although it was initially developed for genomics research, it is largely domain agnostic and is now used as a general bioinformatics workflow management system.
it is also a data integration platform for biological data. It supports data uploads from the user's computer, by URL, and directly from many online resources (such as the UCSC Genome Browser, BioMart and InterMine). Galaxy supports a range of widely used biological data formats, and translation between those formats. Galaxy provides a web interface to many text manipulation utilities, enabling researchers to do their own custom reformatting and manipulation without having to do any programming.
Basically, the Galaxy interface is separated into 3 parts. The tool list on the left, the viewing pane in the middle and the analysis and data history on the right. We will be looking at all 3 parts in this tutorial.

## Getting data into Galaxy¶
There are 2 main ways to get your data into Galaxy. We will use each of these methods for 3 files and then use those 3 files for the rest of the workshop.
Start a new history for this workshop. To do this:
Click on the history menu button (the icon) at the top of the Histories panel.
Select Create New.
It is important to note that Galaxy has the concept of “File Type” built in. This means that each file stored needs to have its type described to Galaxy as it is being made available. Examples of file types are: text, fasta, fastq, vcf, GFF, Genbank, tabular etc.
We will tell Galaxy what type of file each one is as we upload it.

## Method 1: Upload a file from your own computer¶
With this method you can get most of the files on your own computer into Galaxy. (there is a size limit).
Download the following file to your computer: https://swift.rc.nectar.org.au:8888/v1/AUTH_377/public/galaxy101/Contig_stats.txt.gz
        From the Galaxy tool panel, click on Get Data -> Upload File
        Click the Choose File button
        Find and select the Contig_stats.txt.gz file you downloaded and click Open
        Set the “Type” (= file format) to tabular
        Click the Start button
        Once the progress bar reaches 100%, click the Close button
The file will now upload to your current history.

## Method 2: Upload a file from a URL¶
If a file exists on a web resource somewhere and you know its URL (Unique resource location - a web address) you can directly load it into Galaxy.
    From the tool panel, click on Get Data -> Upload File
        Click on the Paste/Fetch Data button
        Copy and paste the following web address into the URL/Text box: https://swift.rc.nectar.org.au:8888/v1/AUTH_377/public/COMP90014/Assignment1/bacterial_std_err_1.fastq.gz
        Set the file format to fastqsanger (not fastqcsanger)
        Click Start
        Once the progress bar has reached 100%, click Close
Note that Galaxy is smart enough to recognize that this is a compressed file and so it will uncompress it as it loads it.
