# IEEEtran Format Template

**Gael Close** | 26-Sep-2022

This is a Quarto template that assists you in creating a manuscript for IEEE Transactions journals and conferences. 
The directory [style-guide](style-guide) contains the reference sample PDF downloaded as part of the [IEEE template selector](https://template-selector.ieee.org/secure/templateSelector/publicationType).
This templates will generate an output with similar formatting.



## Installation For Existing Document

You may use this format with an existing Quarto project or document.
Unzip the content of this repository in the quarto project or document directory.

## Usage

To use the format, you can use the format names `ieeetran-pdf` and `ieeetran-html`. For example:

```bash
quarto render article.qmd --to ieeetran-pdf
```

or in your document yaml

```yaml
format:
  pdf: default
  ieeetran-pdf:
    keep-tex: true    
```

You can view a preview of the rendered template [here](template.pdf).

## Format Options

This format does not have specific format option. 

## Limitations

Currently it only support the `journal` option of the [IEEEtran latex class](https://www.ctan.org/tex-archive/macros/latex/contrib/IEEEtran/).
The `conference` option is not yet supported.

## Dependencies

The [extension latex-environment](https://github.com/quarto-ext/latex-environment) should be installed to support the Markdown table.