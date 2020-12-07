# Useful-Tips
A repository for sharing useful tricks and tools

My suggestion is that we use this as a place to share any useful tricks we learn about duering the semester. Just add them to this README.md file and then send me a "pull request", to ask that your changes are included in this Master version.


# Knitting to HTML file on Github
Problem: Can't find a way to make html markdown outputs look nice on github for a human to read

Solutions:
Change output in the beginning of your rmarkdown file to either
1. output: rmarkdown::github_document
2. output: 
  html_document:
    keep_md: true
3. output: 
  github_document:
    pandoc_args: --webtex
    
Choose whichever you like, but please note that 2 and 3 require new lines (can't seem to output them here). #3 allows you to output latex code properly while the first two do not. All of these will knit a file that ends with ".md" which should be uploaded

# Uploading figure files
problem: Figures do not show on GitHub when you upaod a .md file.

Solutions: The markdown file needs to look the figures up, and they are kept in a separate folder. Go to the folder containing the .md file and find another folder, created at the same time, called something like “figure-gfm”. Upload or commit the folder along with the .md file. It shoudl then find the figures and render them ok.
