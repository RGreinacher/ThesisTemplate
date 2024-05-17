# Thesis Template for Bachelor's and Master's Theses at the QU Lab of TU Berlin

This thesis template provides one possible structure on how to create a thesis at the Quality and Usability Lab.
Additionally, the documents includes useful information on how to structure, write, do references, etc.

This repo is a fork from the original work by [Vera Schmitt](https://github.com/veraschmitt/Thesis_Template). This repo is different in that it promotes a four-chapter structure (Intro / Methods / Results / Discussion).



## How to use it

### Overleaf

For the usage in Overleaf, download the repository first by clicking on <kbd>Code</kbd> and then <kbd>Download ZIP</kbd>

Then, on the overleaf website click on <kbd>New Project</kbd>, <kbd>Upload Project</kbd> and then select the zip archive.

### Using it locally

First, download or clone the repository. With latex installed, run

```
pdflatex main; bibtex main; pdflatex main; pdflatex main
```

This builds your document, including references and bibtex citations. The newly created document is called `main.pdf` and is located in the root folder.



# Explanation of the Overleaf project structure
Here you can change the overall structure of the chapters. If you go to the main file from line 104 on, the structure of the chapters is defined. With the \verb!\input{}! command you can insert the sections from the different folders. The headings of the sections and subsections should be added/defined in the main file not in the respective sub-files for the different chapters. Here the list of figures and tables are added too (line 86). If you add a figure or table in your text it should appear in the list automatically. 

You can add and remove all files very flexible via the main file. Which makes it very flexible and easily to restructure the thesis as you need it. If you do not \verb!0_explanation.tex! file to show up in the text, just remove it in the main file. Similarly you can just remove the  \verb!example.tex! file from the main file. 

If you want to \textbf{comment something out} you can use \verb!%! sign in front of a command or paragraph. 

## Chapter
The different chapters are organized in folders which better structures the thesis project. Just write the text into the different .tex files in the respective folders which you can add and remove via the main.tex file. 

## Figures
In the figures folder you can add all your figures to keep the structure more concise. .png and .pdf are always working, some other formats might cause some errors. 

## References
All your references should be added to the \textbf{ref.bib} file. There are some examples of how to add different formats of citations for inproceedings or books and so forth. See also add the end of the document in chapter 8 how to add references via Google Scholar. For this document the APA citation style is selected, as it makes it more comprehensible for the reader to follow the especially the literature review. If you want to change it, you can change line 63 in the main.tex file to another format.

## Citation
If you want to cite something in the text you have two basic citation commands: \verb!\citet{}! and \verb!\citep{}!. Whereas \verb!\citet{}! will add a citation within the text like "according to Bremner et al. (2019) the model...." and \verb!\citep{}! adds references with parentheses when you do not address the author directly in the text. For more information on the natbib package and its usage please check out this link: \url{https://gking.harvard.edu/files/natnotes2.pdf}.

## Plagiarism
If you take any idea or concept from other sources (independent which kind of source it is) you have to note that. Not only sentences you copy from other work must be denoted with quotation marks or italic in combination with the reference, but also ideas and concepts you paraphrase mus be denoted. Please take the issue of plagiarism serious! For more information on plagiarism and what counts as plagiary please visit: \url{https://ethz.ch/students/en/studies/performance-assessments/plagiarism.html}

## Rest Folder

### Declaration
Here you can find the \textbf{declaration.tex} file which should be signed by you. This is crucial and mandatory for any plagiary related issues. Hereby you state that the thesis is your own work. You can simply add your details in the file directly and if you print out the thesis you can either sign it manually or also with any kind or program you are usually working with.

### Glossary
The \textbf{glossary.tex} file defines all your abbreviations, this is sometimes useful, when you use a lot of abbreviations to collect them in one place, such that the reader can quickly look them up, if he/she has forgotten what the abbreviation means.

You can define all your abbreviations in the \textbf{glossary.tex} file and if you use the abbreviation for the first time in the text than use following command: \verb!\gls{gru}!, this will automatically add the abbreviation GRU in the visible "List of Abbreviations". 
E.g. currently there are many abbreviations in the glossary.tex file but only 2 (\gls{me} and \gls{gru}) are used in the text. only if you use the  \verb!\gls{gru}! command the abbreviation will be shown in the printed file. 

### Title
The \textbf{title.tex} file defines everything on the title page. Here you can add your name and the names of your supervisors, the title and subtitle of your thesis an so forth. The logo of the TU is already added and you actually just need to fill in your data. The date is always the actual date of the day you are working in the document. 

## Long Table
The file \verb!long_table_example.tex! is an example of a very long table and how it can be structured. Please use the predefined style of the tables, as this is the most prominent one in scientific writing. 
