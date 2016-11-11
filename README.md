# すべてのドキュメントを markdown で書こう

客に出す資料とかスライドを markdown で書きたいので  
LaTeX と pandoc を利用して  
markdown から pdf に一発で持っていける環境を用意する  

    sudo pacman -S pandoc texlive-langjapanese texlive-latexextra

# markdown ファイルを一発で pdf にする

    pandoc draft.md -o document.pdf -V documentclass=ltjarticle --latex-engine=lualatex

他にも nodejs-markdown-pdf などのツールもあるが  
いったん LaTeX にしたほうが図の利用や表や注釈など使えてよかった  
それがいらないなら nodejs-markdown-pdf のほうがお手軽だし良いと思う。  
nodejs なので css も使えるしね。  

### 画像で頑張る

グラフとか拾ってこれるものは web から  
作ったものは画像化してとりこむ  

時間があった場合にのみ pdf の体裁をさらに整える  
pdf を inkscape に取り込んで svg 化し  
デザインを整える。  
