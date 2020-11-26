# ice1000's resume

[![GitHub top language](https://img.shields.io/github/languages/top/ice1000/resume.svg)](https://github.com/ice1000/resume)
[![GitHub forks](https://img.shields.io/github/forks/ice1000/resume.svg?style=social&label=Fork)](https://github.com/ice1000/resume)

This is my resume, based on [this template](https://github.com/billryan/resume).
There's a Haskell project to generate the TeX source files, built with cabal (new-style project).

# Build

To build this resume, install texlive-full and GHC toolchain first.<br/>
Then:

```bash
# Install the generator
cabal install --overwrite-policy=always
# Generate the TeX files
resume-gen en >> latex/resume.tex
resume-gen cn >> latex/resume-cn.tex
resume-gen elab >> latex/resume-elab.tex

# Build the TeX files
make -C latex
mv latex/*.pdf .
```

# Download/下载

+ [English simplified version (pdf)](./resume.pdf)
+ [English full version (pdf)](./resume-elab.pdf)
+ [中文版 (pdf)](./resume-cn.pdf)
