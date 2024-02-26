---
layout: default
title: "MD to PDF"
permalink: MD-PDF-survey
---

# MD to PDF conversion survey

## Available tools

* [Pandoc](https://pandoc.org/)
* [wkhtmltopdf](https://wkhtmltopdf.org/)
* [WeasyPrint ](https://github.com/Kozea/WeasyPrint)
* [mdpdf](https://github.com/BlueHatbRit/mdpdf)
* [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf)
* [markdown-pdf](https://github.com/alanshaw/markdown-pdf)

## Installation script

These commands and tools have been tested on Ubuntu 20.04 LTS and Ubuntu 22.04 LTS, but some does not work on both.

```bash
# Update
sudo apt update
sudo apt upgrade -y
sudo apt autoremove -y

# Install Python and Pip
sudo apt install -y python3 python3-pip
python3 -m pip install -U pip

# Install NodeJS and NPM
sudo apt install -y npm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
source ~/.bashrc
nvm install --lts

# Install Pandoc and LaTeX
sudo apt install -y pandoc texlive-latex-extra texlive-lang-french

# Install wkhtmltopdf
sudo apt install -y wkhtmltopdf

# Install weasyprint
pip install weasyprint

# Install mdpdf
npm install mdpdf --global

# Install md-to-pdf
npm install md-to-pdf --global

# Install markdown-pdf
npm install markdown-pdf --global
```

## Conversion Makefile

```makefile
all: pandoc clean


tmp.html: file.md
	pandoc $< --output=$@


pandoc: file.md
	pandoc $< --output=$@.pdf --metadata-file .header.yml

wkhtmltopdf: tmp.html
	wkhtmltopdf --encoding utf-8 $< $@.pdf

weasyprint: tmp.html
	weasyprint --encoding utf-8 $< $@.pdf

mdpdf: file.md
	mdpdf $< $@.pdf

md-to-pdf: file.md
	cat $< | md-to-pdf > $@.pdf

markdown-pdf: file.md
	markdown-pdf $< --out $@.pdf


clean:
	rm -f tmp.*

clear: clean
	rm -f *.pdf
```

This Makefile is inspired from [this repo](https://github.com/Relex12/Decentralized-Password-Manager/blob/master/readme/Makefile), you can clone it and give it a try.
