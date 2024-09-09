# LaTeX

**LaTeX** (pronounced “LAY-tek” or “LAH-tek”) is a tool for creating professional-looking documents. Unlike programs like Microsoft Word or LibreOffice Writer, where you type and style text directly on the page, LaTeX works differently. You write your document as a plain text file with special commands to format it. Read more about typesetting here:  [https://www.overleaf.com/learn/latex/Learn\_LaTeX\_in\_30\_minutes](https://www.overleaf.com/learn/latex/Learn\_LaTeX\_in\_30\_minutes)

See here for a LaTeX cheat-sheet, including most commonly used commands.&#x20;

{% file src="../.gitbook/assets/latexsheet.pdf" %}

### **Templates**

There are templates available for academic conference and journal papers, many of which are available on the Overleaf templates page. The final report template we recommend is here:  [https://www.overleaf.com/latex/templates/ieee-conference-template/grfzhhncsfqn](https://www.overleaf.com/latex/templates/ieee-conference-template/grfzhhncsfqn)&#x20;

If you prefer to use a local installation, see below for a .zip file containing the IEEE 4 page conference paper template for the report. Please do this at your own risk, we highly recommend using Overleaf otherwise:

{% file src="../.gitbook/assets/IEEE Conference Template.zip" %}

**Tips**

Quotation marks are a bit tricky, please use \`\` instead of ''.

\ is a special 'escape' character (bonus points if you are familiar with C strings for the reference), and many symbols you would like to include in the text will depend on proper usage of the backslash.&#x20;

The $ sign is used to format mathematical content, and can be used in-text too. Please consider using these while including any numbers, equations, or simple formulae which are not within the equation space.

Please also consider using the \centering command while including graphics and tables, so they are properly justified.&#x20;

Please also consider using the \cite, \label and \ref commands appropriately while citing papers or resources from the references, and also pointing to other parts of your report (refer to Section \ref{section-one}, where "section-one" is properly labeled, for example).

If you have tables in the report, please consider using this table generator instead of hand-rolling one: [https://www.tablesgenerator.com/#google\_vignette](https://www.tablesgenerator.com/#google\_vignette)&#x20;

We require that anything you use from other papers/resources online are appropriately cited. We recommend using a citation manager like Mendeley, which works very well [with Overleaf](https://www.overleaf.com/learn/how-to/How\_to\_link\_your\_Overleaf\_account\_to\_Mendeley\_and\_Zotero).

This is the easiest (if you find an easier way, let us know!) way to work with references as a group as well. Alternatively, [bibtex](https://www.overleaf.com/learn/latex/Bibliography\_management\_with\_bibtex) is the traditional way, which works quite well when [exported from Google Scholar](https://digitalmeasures.oregonstate.edu/training/export-bibtex-google-scholar).&#x20;

