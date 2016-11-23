# Equity Transfer Caps Extension

The equity transfer caps extension provides a way to descibe the limits defined in the contract on the transfer of equity in the project company.

Modelling this information as structured data is important so that users can compare the equity transfer caps in different projects and jurisdictions.

This extension introduces the following new elements to the OCDS schema:

* An ```equityTransferCap``` building block
* A ```milestoneReference``` building block
* An ```equityTransferCaps``` field to the ```contract``` section of OCDS

## Equity Transfer Caps Field

The ```contract/equityTransferCaps``` field is an array of ```equityTransferCap``` building blocks, describing the caps on equity transfer in the contract.

## Equity Transfer Cap Building Block

The equity transfer cap building bock provides a way to:

* Provide a free text title and description for the cap
* State the maximum amount of equity that can be transferred under the cap
* Describe the period for which the cap is effective by linking to a milestone

```eval_rst
.. extensiontable::
   :extension: equityTransferCaps
```

## Milestone Reference Building Block

The milestone reference building block provides a way to references milestones described elsewhere in the contracting process using the ```ID``` and ```title``` of the milestone.