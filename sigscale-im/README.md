# SigScale RIM
This application is used by communications service providers (CSP)
for Resource Inventory Management (RIM). It provides the TMFC010
and TMFC012 Components of the TM Forum Open Digital Architecture
(ODA), producing the TMF639 and TMF634 Open APIs.

## Resources
The information model is based on TM Forum SID and 3GPP Network
Resource Models (NRM). The catalog is populated with specifications
representing the entities of the 3GPP NRMs as well as ETSI MEC
and TM Forum ODA.  The inventory contains dynamically created
representations of the intantiated resources provided by this
software application, obtained through self relection.

## REST
The core functions of the TMFC010 and TMFC012 ODA Components
produce the TMF634 and TMF639 Open APIs. Supported operations
include creating resource inventory, creating resource
specifications and querying inventory and catalog with TMF630
Part 6 advanced query patterns (JSONPath).

### Progressive Web App (PWA)
A human interface is also provided as a stanadlone PWA which
simply uses the TM Forum Open APIs while providing a visually
pleasing presentation. This provides a convenient table form
with expanding details and tabbed views to make browsing the
catalogs and inventories easy.
![screenshot](https://raw.githubusercontent.com/sigscale/rim/master/doc/specifications.png)

