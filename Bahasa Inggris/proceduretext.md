# How to write in LaTeX
> This is a MASSIVE OVERSIMPLIFED tutorial of LaTeX that I used to do my english assignment. If you want to learn more abour LaTeX, just use google or to https://www.overleaf.com/learn/latex.

LaTeX (pronounced LAY-tek or LAH-tek) is a tool used to create professional-looking documents. In order to create a LaTeX document, first you'll need:
- PC
- Overleaf Account (register on https://www.overleaf.com/register)
- Keyboard

Second, open your Overleaf account and create new project. You will see a two separate window in your monitor. The left one is called the "Code Editor" and the right one is called the "PDF Viewer". You will mostly working with the code editor, so clicked the window on the left.

Third, if there's no text inside the code editor, you'll need to write this command:
```latex
    \documentclass{article}

    \begin{document}

    \end{document}
```
After that, you can insert your own text below '\begin{document}' and above '\end{document}' like this:
```latex
    \documentclass{article}

    \begin{document}
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque et mollis dui. Ut vitae nisl imperdiet, aliquam nisl in, sagittis nunc. Quisque nec nunc ut tortor interdum venenatis a a sapien. Vivamus felis orci, convallis sit amet mollis eget, aliquet sit amet velit. Vestibulum consequat rhoncus magna, sed tincidunt ante accumsan sed. Praesent suscipit blandit imperdiet. Nam rhoncus sem eu commodo laoreet. Duis finibus diam at enim eleifend consequat.
    \end{document}
```

Fourth, to see the results of your document, you can press CTRL-S or click "Recompile" button above the PDF Viewer. Then you will see your document in PDF.

There's so many features that LaTeX has including support for external images, mathematical equations, etc; and really useful if you want to create a scientific journal or academics paper. You can learn more about LaTeX in https://www.overleaf.com/learn/latex.