# Let's write all documents markdown

I'd like to write materials and slides to customers for markdown  
Using LaTeX and pandoc Prepare an environment that you can have in one  
shot from markdown to pdf  

    sudo pacman -S pandoc texlive-langjapanese texlive-latexextra

# Make the markdown file pdf with one shot

    pandoc draft.md -o document.pdf -V documentclass=ltjarticle --latex-engine=lualatex

    sudo pacman -S poppler poppler-data inkscape
