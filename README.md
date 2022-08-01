# ArXiV Template

This is a Quarto template that assists you in creating PDF outputs which closely match those published on arXiv. If you are intending to publish your article on arXiv, it is highly recommended you upload your TeX files (and supporting files, including generated `.bbl` and figure files) directly. However, this template supports rendering PDFs which resemble arXiv preprints for upload to other repositories either before or instead of submission to arXiv itself.

Please note this template should be considered an early alpha as I work out a few mismatches between the current output and the arXiv style.

## Creating a New Article

You can use this as a template to create a preprint for ArXiV. To do this, use the following command:

```quarto use template mikemahoney218/quarto-arxiv```

This will install the extension and create an example qmd file and bibiography that you can use as a starting place for your article.

## Installation For Existing Document

You may also use this format with an existing Quarto project or document. From the quarto project or document directory, run the following command to install this format:

```quarto install extension mikemahoney218/quarto-arxiv```

## Usage 

To use the format, you can use the format names `arxiv-pdf` and `arxiv-html`. For example:

```quarto render article.qmd --to arxiv-pdf```

or in your document yaml

```yaml
format:
  pdf: default
  arxiv-pdf:
    keep-tex: true    
```

You can view a preview of the rendered template at <https://quarto-journals.github.io/quarto-arxiv/>.

