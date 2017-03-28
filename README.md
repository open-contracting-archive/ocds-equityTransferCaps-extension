# Equity Transfer Cap extension

This extension was proposed in order to model a requirement in the [World Bank PPP Disclosure Framework](http://pubdocs.worldbank.org/en/773541448296707678/Disclosure-in-PPPs-Framework.pdf) to record information on 'equity transfer caps'.

These are present in some complex Public Private Partnership projects, where a shareholder may have restrictions on how much equity they can sell or exchange until particular project milestones are met.

This was initially modelled as an object as part of ```contract```. However, evaluation has found that:

* Equity transfer caps would be better modelled as a property of shareholders in a project;
* Any structured data model is likely to have considerable complexity (as caps can be conditional on various milestones or other considerations), and so we should focus on capturing descriptive rather than structured information at this point in time;

As a result, we've abandoned this extension, and suggest including equity transfer cap information:

(a) In associated documentation blocks;

(b) In notes against [shareholders](https://github.com/open-contracting/ocds-shareholders-extension)
