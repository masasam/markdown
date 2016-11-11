# すべてのドキュメントを markdown で書こう

客に出す資料とかスライドを markdown で書きたいので  
markdown から pdf に一発で持っていける環境を用意する  

    sudo pacman -S pandoc texlive-langjapanese texlive-latexextra

# markdown ファイルを一発で pdf にする

    pandoc draft.md -o document.pdf -V documentclass=ltjarticle --latex-engine=lualatex

