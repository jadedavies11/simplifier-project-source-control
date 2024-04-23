### {{page-title}}
Each profile description includes _Mandatory_ and _Must Support_ elements. 

In order to be compliant, when an element is mandatory (min=1), the data is expected to always be present - i.e. **SHALL** be present. Figure 1 below shows how _Mandatory_ elements are presented in the Snapshot View. 
<br><br>
**Figure 1: Mandatory Elements**
{{render:Diagrams-Guidance-MandatoryElements}}
<br>

Elements marked with an <span style="background-color:red;color:white;">S</span> must be supported. While the definition of _Must Support_ is quite general, this implementation guide defines it to mean that provider **SHOULD** populate these elements where possible, and consumer systems **SHOULD** act on this information if provided.

In the case of the `Oganization.active` element, _Must Support_ would mean, for example:
* A provider system would be expected to provide the relevant indicator to show if the organisation is still active.
* A consuming  system would be expected to act on this information and not include an organisation marked as inactive within a list of active organisations.

Figure 2 below shows how _Must Support_ elements are presented in the Snapshot View. 
<br><br>
**Figure 2: Must Support Elements**
{{render:Diagrams-Guidance-MustSupportElements}}
<br>
