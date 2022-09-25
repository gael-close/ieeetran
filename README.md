# IEEEtran Format Template

This is a Quarto template that assists you in creating a manuscript for IEEE Transactions journals and conferences. 
The directory [style-guide](style-guide) contains the reference sample PDF downloaded as part of the [IEEE template selector](https://template-selector.ieee.org/secure/templateSelector/publicationType).
This templates will generate an output with similar formatting.

## Creating a New Article

You can use this as a template to create an article. To do this, use the following command:

```bash
quarto use template quarto-journals/ieeetran
```

This will install the extension and create an example qmd file and bibiography that you can use as a starting place for your article.

## Installation For Existing Document

You may also use this format with an existing Quarto project or document. From the quarto project or document directory, run the following command to install this format:

```bash
quarto install extension quarto-journals/ieeetran
```

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

You can view a preview of the rendered template at <https://quarto-journals.github.io/ieeetran/>.

## Format Options

This format does not have specific format option. 

## Limitations

Currently it only support the `journal` option of the [IEEEtran latex class](https://www.ctan.org/tex-archive/macros/latex/contrib/IEEEtran/).
The `conference` option is not yet supported.