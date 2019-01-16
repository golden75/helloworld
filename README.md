## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/golden75/helloworld/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

```R
# Load DESeq2 library
library("DESeq2")

# Set the working directory
directory <- "~/Documents/R/DESeq2/"
setwd(directory)

# Set the prefix for each output file name
outputPrefix <- "Listeria_DESeq2"

# Location of deseq ready count table (EDGE-pro output)
deseqFile <- "~/Documents/R/DESeq2/Listeria_deseqFile"

# Read the table
countData <- read.table(deseqFile, header = T)

# Replace accession numbers with meaningful names
names(countData) <- c("10403S Rep1","DsigB Rep1","10403S Rep2","DsigB Rep2")

# Create table with treatment information
sampleNames <- colnames(countData)
sampleCondition <- c("10403S","DsigB","10403S","DsigB")
colData <- data.frame(condition = sampleCondition)
row.names(colData) = sampleNames
treatments = c("10403S","DsigB")
```

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/golden75/helloworld/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


### New Added   

this is newly added section to test
