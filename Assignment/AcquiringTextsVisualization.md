
---
title: Assignment 2
author: Wesley Raabe
date: July 28, 2014
bibliography: Assmt2.bib
csl: mla.csl
---


# Acquiring and Visualizing Texts

Our second course project, again collaborative, will be to explore ways of acquiring digital texts and ways of visualizing them.  We could assume that most texts that we want are already available online, but that would be a mistake. More recently published texts, which are still in copyright, may not be available or may only be available in a form in which we cannot copy and paste or grab the text. Therefore, if we want to analyze or visualize a text, we may need to acquire the text either by using optical character recognition software or (god forbid) by transcribing a text manually. In some cases, such as handwritten letters that have not been published, manual transcription may be the best choice. But an online text may not be reliable: it could be abridged (shortened) or censored. One of the reasons for this assignment is to become better aware of how access and visualization, which seem to offer useful and straightforward technological shortcuts to interpretation, are themselves challenging both in a technical sense and as tools for interpretation. 

In this project, we are going to analyze Louisa May Alcott's *Hospital Sketches* to see how tools for visualization can help us devise interpretive readings. That is, we're going to consider what texts are publicly available and how we might visualize them. And then we're going to see how we can improve the quality of our work by being more conscientious and systematic. One version of the text, which was published initially in a Boston newspaper, is not presently available online. So we're going to test methods for acquiring it, including OCR and transcription. Don't worry: we'll break up the work so no one person has to do too much.  

These are the basic processes about which we will gain basic competence during this three-week project:

  -  Acquiring an online version of a text and using systematic methods (text comparison and REGEX) to improve the quality of the transcription.
  -  Using OCR to acquire a text
  -  Using transcription to acquire a text
  -  Using methods to establish likely provenance (source) for a text that lacks identifying information about its origin
  -  Visualizing texts with concordances, word clouds, and text comparison tools to correct and to display differences
  -  Developing sensible procedures for determining what counts as significant and normalizing a text according to those guidelines (this may require you to clean up a text a second time, after you have developed more accurate assumptions about its faults). 
  -  Analyzing the strengths and weaknesses of visualization to support interpretive readings
  
 ## Step 1
 
 When Alcott's publisher Roberts Brothers told her that they wanted to publish a new version of *Hospital Sketches* and some of her war stories, they requested some changes . She described the publisher's requested alterations in her journal: "Arranged 'Hospital Sketches and War Stories' for a book. By taking out all Biblical allusions, and softening all allusions to rebs, the book may be made 'quite perfect,' I am told. Anything to suit the customers" (*Journals* 164). According to scholar Ruth Berman, Alcott (or her publisher) also "cut out most allusions to liquor" ('Spirituous Consolation' 184). In order to assess these details for ourselves, to learn how technological means can be used to identify and review them, our first task is to acquire the two versions of the text, to review them for OCR errors, and to use REGEX with find-replace to correct them when possible. Our purpose is not necessarily to produce a perfect transcription but to reduce the number of incidental errors so that we can focus on the significant, textual changes that can likely be attributed to Alcott's revision or her publisher's censorship.  
 
 *Caution*:  When correcting a text with REGEX, one can often assume a pattern is predictable. And often it is. But errors in our REGEX expression or errors within our assumptions may lead to corruption of the text added by our ministrations.  Therefore, it will be important to be systematic and keep a copy of the original record and of each significant revision---because errors in our processes may require us to go back to a previous version and repeat our work. As is said in software development, this is not a "bug" but a "feature": iterative processes, repeating the same task but refining the methods, can help us learn to do the task better. Also, carefully refining processes can help us to develop a more refined model of how texts are constructed.  
 
1.  Download the Redpath version (1863) of *Hospital Sketches* from the Internet Archive at the following address: [https://archive.org/details/hospitalsketches00alcorich](https://archive.org/details/hospitalsketches00alcorich). Display the "Full Text" option: drag cursor from top to bottom until entire text is selected, or save as text and remove the extraneous detail. Using your favorite text editor, save it into a clearly labeled folder, such as `LMA_HospSketches` as a plain text document. Label it clearly as the initial version with file name, such as `LMAHS_Redp63_InetArc_FullText_ver1.txt.`

2.   Repeat previous step for the Roberts Brothers version (1868) of *Hospital Sketches; and, Camp and Fireside Stories* at the following address: [https://archive.org/details/hospitalsketche00alco](https://archive.org/details/hospitalsketche00alco). Save this file to same folder `LMA_HospSketches` with an unambiguous file name, such as `LMAHS_RobertsBros1868_InetArch_FullText_ver1.txt` Note the significant difference in file size, approximately 170 KB for the Redpath versus approximately 640 KB for the Roberts Brothers. That's because the section entitled "Camp and Fireside Stories" in the Roberts Brothers edition begins on page 97. Delete the other stories, from the appearance of "CAMP AND FIRESIDE STORIES" on page 97 through the end of the text. Save again as `LMAHS_RobertsBros1868_InetArch_FullText_ver1.txt`.

3.   Save both texts as "ver2.txt" in the same folder. Close the "ver1.txt," and open the "ver2.txt" version of each. 

4.   See "Cleaning up OCR with Regular Expressions." As often as prudent save an updated copy of the text as "ver2.txt," "ver3.txt," "ver4.txt." etc. If at any time you notice that a previous "Replace All" had unexpected results or you inadvertently corrupted the file beyond repair, go back to a previous version of the file that you are confident is in good shape. The option to to UNDO previous commands (most text editors allow multiple UNDO routines since last save) should prevent the need to be obsessive about it.   


 ## Reviewing Text Quality

The second step is to analyze the quality of the acquired texts to see whether they will serve our purposes or whether we need to perform additional steps to clean them up. There are numerous tools that you can use to do this. I suggest any one of the following:
 
 - Beyond Compare (Windows, with 30-day trial)
 - WinMerge (Windows, free)
 - DeltaWalkter (Macintosh, $39 license, [http://www.deltopia.com](http://www.deltopia.com))
 - DiffMerge (Macintosh, free)

When comparing texts, you will notice many common OCR problems. Some include the following:

 - Many problems with ligatures (two letters linked together as one): fi, fl, ff, ffi
 - "cl" for "d," and vice versa
 - "u" for "n"," and vice versa
 - "c" or "o" for "e", and vice versa
 - "ni" or "rn" for "m" and vice versa
 - "h" for "b" and vice versa
 - "li" for "h" and vice versa
 - "rm" for "nu" and vice versa

Damage to type descenders (g, y), poor inking, and spots on page will also produce errors, as will spots on microfilm reproductions.  

If you can discern a pattern of error, consider using REGEX to repair. But do check against original images. 
 
 
 ## Step 4?
 Because Alcott's journal statement has been known, most classroom editions print the 1863 version as the less censored Civil War text.  But there is also an earlier version of the story, which was published in a Boston newspaper *The Commonwealth* during the war. We know that the newspaper version is shorter because in the "Publisher's Advertisement" the sketches are described as "revised and enlarged" (5). 
  
  

 




# Bibliography

	
	