# Section 1: Should I publish in the USLCI?  

[**_Return to TOC_**](./00-sub-handbook-landing.md)

This page provides a high-level explanation of the benefits, expectations, and general process for publishing data on the [U.S. Life Cycle Inventory Database (USLCI)](https://uslci.lcacommons.gov/uslci/search). This Submission Overview is intended to help interested parties understand the benefits of publishing their data on the USLCI and set reasonable expectations for the publication documentation and standards.   


This page is divided into the following subsections.
1. [**Benefits**](./01-should-i-publish-in-the-uslci.md#benefits)
2. [**Expectations**](./01-should-i-publish-in-the-uslci.md#expectations)
    * [_Placing your data in the public domain_](./01-should-i-publish-in-the-uslci.md#placing-your-data-in-the-public-domain)
    * [_Dataset citations_](./01-should-i-publish-in-the-uslci.md#dataset-citations)
    * [_Data formatting_](./01-should-i-publish-in-the-uslci.md#data-formatting)
3. [**Data requirements**](./01-should-i-publish-in-the-uslci.md#data-requirements)
    * [_Data reliability and reproducibility_](./01-should-i-publish-in-the-uslci.md#data-reliability-and-reproducibility)
    * [_Categorization_](./01-should-i-publish-in-the-uslci.md#categorization)
    * [_Nomenclature_](./01-should-i-publish-in-the-uslci.md#nomenclature)



<a id="benefits"></a>
## Benefits

LCA serves as a benchmarking and comparison tool for sustainable product and process development. As public and private actors increasingly utilize LCI data for decision-making and communications along the value chain, LCI data availability, reliability, and geographic specificity become increasingly important. The USLCI Database offers data providers with the opportunity to share complete, representative, and well-documented LCI data to a public repository. This resource allows users with influence across the value chain access to transparent and representative LCI data alongside guidance for its intended use. The goals of the USLCI Database are to maintain data quality and transparency, support the use of LCA, maintain compatibility with other LCI databases, provide exceptional data accessibility, be fully and sustainably supported, and support US industry competitiveness.

NREL is collaborating with the [US Department of Agriculture (USDA)](https://www.usda.gov/) the [Environmental Protection Agency (EPA)](https://www.epa.gov/), the [National Energy Technology Library (NETL)](https://www.netl.doe.gov/), the [Argonne National Laboratory (ANL)](http://www.anl.gov/), the [US Army Corps of Engineers (USACE)](https://www.usace.army.mil/), the [Federal Highway Administration (FHWA)](https://www.fhwa.dot.gov/), the [US Forest Service (USFS)](https://www.fs.fed.us/), the [Federal Aviation Administration (FAA)](https://www.faa.gov/), and the [National Institute of Standards and Technologies (NIST)](https://www.nist.gov/) to develop a US Federal LCA Data Commons. This ongoing effort endeavors to provide improved and coordinated access to Federal LCA data. 

<a id="expectations"></a>
## Expectations

The USLCI provides individual gate-to-gate, cradle-to-gate and cradle-to-grave accounting of the energy and material flows into and out of the environment that are associated with producing a material, component, or assembly in the US. These data are intended to cover commonly used materials, products, and processes in the US with up-to-date, critically reviewed LCI data.  

<a id="placing-your-data-in-the-public-domain"></a>
### Placing Your Data in the Public Domain

To support increased access to and sharing of scholarly resources, as well as to promote novel and innovative uses of LCA data, NREL requires that all datasets submitted to the LCA Commons be placed in the public domain under the terms of the [Creative Commons Legal Code (CC0 1.0 Universal (CC0 1.0))](./04-resources/04-App-C.md). By placing your datasets in the public domain, according to the CC0 1.0 license, you are removing “all of [your] rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law.” Please review the legal code of the CC0 1.0 Universal license before submitting your datasets, as well as the [Data Use Disclaimer Agreement (“Agreement”)](./04-resources/04-App-A.md) and [Data Provider’s Content License Agreement (“Agreement”)](./04-resources/04-App-A.md).

<a id="dataset-citations"></a>
### Dataset Citations

Individuals who use USLCI datasets from the LCA Commons should cite these datasets to acknowledge and credit the work of data creators. For example, "Data Generator (2018). Dataset Name, US Life Cycle Inventory Database." National Renewable Energy Laboratory (NREL), 2018. Accessed April 15, 2018: [https://www.lcacommons.gov/nrel/search](https://www.lcacommons.gov/nrel/search).

<a id="data-formatting"></a>
### Data Formatting

The International Organization for Standardization (ISO) specifies data documentation formats for LCA in [ISO/TS 14048:2002](https://www.iso.org/standard/29872.html).

![](https://github.com/uslci-admin/private-uslci-content/blob/dev/images/ISO%2014048%20-%20Graphic.png)
**_ISO 14048 LCA Data Documentation Format Concepts_**   
<br>
<br>

To facilitate compliance with this standard, the LCA Commons is structured upon the [openLCA](http://www.openlca.org/download/) database schema<sup>[**[1]**](#fn1)</sup>, which includes the elements designated in the above figure. To minimize data formatting efforts and ensure all metadata elements persist throughout submission, unit process and product system datasets submitted to the USLCI Databaes/LCA Commons should be edited in openLCA. If you already work in a version of openLCA, discuss this with the NREL Data Curator at the beginning of the data submission process to ensure compatibility.

Editing guidance is provided in the Ingest & Onboarding and Guidance on Data Compilation in openLCA sections of this handbook. Once you edit your Unit Processes or product systems in openLCA, you may share them through your institutional repository hosted by NREL as exported JSON-LD files. NREL will then publish the data to its internal repository. The openLCA software can be downloaded free of charge at openLCA.org.

EcoSpold (v1 and v2) and International Reference Life Cycle Data (ILCD) submissions generated by SimaPro, GaBi, ecoEditor, the ILCD editor, or any other editor may not support required metadata fields, and datasets may be returned to you. Please import and edit these datasets in openLCA and export files in the openLCA JSON-LD file format for submission. Inspecting your data in openLCA prior to submission is an opportunity to preview how your data will appear in the LCA Commons. Alternatively, if your work is in spreadsheets, you can use the openLCA spreadsheet format to import your data into the openLCA desktop application and then edit in openLCA.

Detailed guidance on the data submission process is covered in Section 2: How do I publish my data in the USLCI?   

<a id="data-requirements"></a>
## Data Requirements

The LCA Commons will accept both unit process (i.e., ‘gate-to-gate’) and product system (i.e., ‘cradle-to-gate’ or aggregated) models. While it is preferred to have the data in a gate-to-gate format to support transparency of data, it is understood that a certain level of aggregation may be required to protect confidential data. In these cases, it is requested to aggregate only as much as needed to protect the data. Some data providers have been providing their data in both a system’s level dataset (fully aggregated) as well as a gate-to-gate format. This approach allows those users who prefer to utilize the systems level dataset and those who want to be able to do certain scenario modelling to use the gate-to-gate versions. Any aggregated or product system datasets must include documentation stating the type of and motivation for the aggregation (e.g., horizontal averaging, vertical aggregation; proprietary, ease-of-use)<sup>[**[2]**](#fn2)</sup>. 

Multi¬functional unit processes should include all co-products and may also include allocation factors or displaced products (according to the discretion of the submitter). The allocation approach should be justified and clearly described. Unit processes may be submitted as single gate-to-gate processes, or related processes grouped as product or intermediate product systems. If multiple unit processes for a product system are submitted, the linking between them should be explicit.

<a id="data-reliability-and-producibility"></a>
### Data Reliability and Reproducibility

Flow data within the unit process(es) must be based on measurements using a specified and standardized measurement method OR estimated using methods and data described in specified archival or other publicly available sources. Furthermore, data should represent a novel contribution (i.e., unique process, unique market, update, and dataset does not duplicate existing data) to the LCA community and be non-proprietary. If the data are an update to a previously published dataset, a note will be added to the metadata of the unit process dataset (i.e., see: the [Administrative Information Field Conventions Table](./field-conventions/admin-info.md) _‘Intended Application’_ field of the [‘Administrative Information’ tab)](./field-conventions/admin-info.md#admininstrative-information)). Unit processes that represent proxy upstream processes from external databases should not be submitted (e.g., ecoinvent process datasets).

<a id="categorization"></a>

### Categorization
Flows are categorized as either elementary or technosphere flows. Datasets from different databases with disparate categorization schemes can prevent connectivity, cause duplications and/or confusion among users, and result in a bulky database.

Technosphere flows and intermediate processes are classified using the North American Industry Classification System (NAICS) 2 digit/4 digit classification scheme for categorizing intermediate processes and technosphere flows (see: https://www.census.gov/eos/www/naics/). Please ensure that your datasets are submitted using this format and reflect the latest NAICS updates, which occur roughly every three to four years.

A technosphere flow that is not being submitted as a dataset and is not already in the USLCI or another repo of the FLCAC should be categorized in the _Technosphere Flows>CUTOFF Flows_ folder with the description 'CUTOFF' in the product flow description metadata. Otherwise, a reasonable proxy from the USLCI may be identified with a note in the _‘Input Flow, Description’_ field regarding the flow provenance (database origin and original flow name). Processes from other databases should not be submitted as datasets.


<a id="nomenclature"></a>
### Nomenclature

Detailed guidance on process and flow nomenclature for USLCI are provided in [Table 1. General Information Field Conventions](./field-conventions/general-info.md#general-information) of the [Metadata Guidance Tables](./02-how-to-publish-in-the-uslci.md#metadata-guidance-tables) and [Appendix D: ILCD Nomenclature Rules](./04-resources/04-App-D.md). 

##### Technosphere Flows
Intermediate flows are are either products or processes from the technosphere (i.e., not elementary flows).

Intermediate product flows are technosphere flows that are a product of one or more processes and have flowable names and flow properties. Technosphere or product flows are the result of a process (or processes) and flow as exchanges between processes (unlike elementary flows that flow as exchanges to and from environmental compartments). All intermediate product flow names should be decoupled from their associated activity flow names (i.e., process name) for transparency and clarity. That is, a product name should not contain metadata that is specific to the activity context such as the location or year. The intermediate product name should be generic to any activity context so as to avoid unnecessary duplication of product flow names. Likewise, product flow properties such as units, formulas, synonyms, infrastructural flow designation, etc. may be defined in the metadata and should also not be included in the flowable name.

An intermediate process is an activity containing at least one intermediate product flow. Activities are exchanges containing at least one input flow and one output flow (i.e., defining a relationship between flows). The intermediate process flow name should reflect the product or service it represents; the product reference output is given the same name as the process name; the naming conventions are as follows: Base name; treatment, routes, standards; production type, location type; quantitative flow properties. The base name is a general descriptive name of the process using technical language. The technical name should be given as it is used in the respective industry or toward their customers. The standards include qualitative information about the process in technical terms (see Rules 1-19 Appendix E: ILCD Nomenclature Rules or the full ILCD Handbook for a list of potential descriptive terms). The quantitative process properties further specify information on process in technical quantitative term(s).

Data curation services will include integrating data sets into internally consistent linked data products for intermediate flows having default providers within the Federal LCA Commons repositories (e.g., USLCI background data, Electricity Baseline, Heavy Equipment). To reference intermediate flows from another database (e.g., ecoinvent(R), GaBi, Quantis, Agri-footprint), the flow names, i.e., nomenclature should match the original database exactly in the 'Input, Flow' field and indicate provenance in the 'Input, Flow, Description' field). These outside database flow references will be submitted as 'Cutoffs' with reference to the provenance such that they may be re-integrated by end-users. This data set integration must occur locally by the data provider prior to submitting the sets to USLCI for curation.  Processes from other databases (i.e., already existing outside the FLCAC) should not be submitted as datasets. As mentioned, a technosphere flow that is not being submitted as a dataset and is not already in the FLCAC should be categorized in the Technosphere Flows\ ‘CUTOFF’ folder or a reasonable proxy from the FLCAC identified with a note in the ‘Input Flow, Description’ field regarding the flow origin (database and flow name). 

Additional guidance on the ILCD nomenclature for technosphere and process nomenclature can be located in the [ILCD Nomenclature Rules Appendix](https://github.com/uslci-admin/uslci-content/blob/dev/docs/submission_handbook/04-resources/04-App-D.md) of this Handbook or the [ILCD Handbook](https://eplca.jrc.ec.europa.eu/uploads/MANPROJ-PR-ILCD-Handbook-Nomenclature-and-other-conventions-first-edition-ISBN-fin-v1.0-E.pdf).

##### Elementary Flows
Elementary flows are data components of LCA data that describe common physical items that move from the technosphere into nature or vice versa. They are used in exchanges in life cycle inventory (LCI) data to represent these movements into and out of processes, and they are used in Life Cycle Impact Assessment (LCIA) methods to match inventory data with impact characterization factors. Hence, they serve a critical role in LCA modeling and are essential in achieving LCA data interoperability.

The US EPA has developed a master elementary flow list (the FEDEFL), which is available in CSV and openLCA schema JSON-LD formats, and provides resources to help with mappings. The current release version is available via the [FLCAC portal](https://www.lcacommons.gov/lca-collaboration/#). The USLCI has adopted the EPA Federal LCA Commons Elementary Flow List (FEDEFL) for elementary flow classification. Elementary flows are further classified into eight classes as described in the [FLCAC Guidelines Appendix D: Highlight 4](https://github.com/uslci-admin/uslci-content/blob/dev/docs/submission_handbook/05-FEDEFL%20Guidelines%20-%20Appendix%20Fork.md). The classification of elementary flows employed by the FEDEFL allows for a systematic approach for managing elementary flows on the Federal LCA Commons. Additional guidance on using and converting to this nomenclature can be found on the [FEDEFL github repository wiki page](https://github.com/USEPA/Federal-LCA-Commons-Elementary-Flow-List/wiki) or the [FEDEFL guidance document](https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=341199). The FEDEFL wiki provides guidance on converting an established flow list in a standard openLCA format to FEDEFL flows. Please see the US EPA report, [The Federal LCA Commons Elementary Flow List: Background, Approach, Description and Recommendations](https://cfpub.epa.gov/si/si_public_record_Report.cfm?dirEntryId=347251&Lab=NRMRL) for Use for more information regarding the FEDEFL requirements and nomenclature.

When submitting data, the elementary flow names in the LCI must correspond directly to the elementary flow names used in the LCIA method. Usage of the FEDEFL protocol for both LCI and LCIA datasets on the FLCAC ensures interoperability between these different types of datasets and the original and FEDEFL names are documented during the curation process.

To assist with transition to the FEDEFL, document LCIA methods used in the ‘Intended Application’ field of the Administrative Information tab in openLCA. If data being submitted have NOT been used in an LCIA, please use flows from the openLCA reference list. If you used SimaPro or GaBi modeling software and an impact method that is also provided for in the openLCA suite of LCIA methods, please run your inventory and impact results in openLCA and compare them to those obtained in SimaPro or GaBi to confirm that openLCA is reading flows correctly.



### Data Quality Scheme

Within openLCA, the only data quality scheme available by default is that of ecoinvent®. Publishing agencies may have developed their own scheme and still, some may not use a scheme at all. The FLCAC does not require a specific scheme be utilized; however, there is guidance in this document on how to utilize the EPA Data Quality Pedigree Matrix if it is elected. The USLCI uses the EPA Data Quality Pedigree Matrix (downloaded and imported into openLCA from the GreenDelta downloads page).

<br><br>


<a id="fn1"></a>
>[1](#data-formatting). This requirement exists to enable data transfer and does not imply an official endorsement of openLCA as a life cycle modeling tool.

<a id="fn2"></a>
>[2](#data-requirements). For more information regarding motivations for data aggregation, see: Table 3.1 Motivations for aggregated datasets, UNEP/SETAC 2011 Global Guidance Principles for Life Cycle Assessment Databases: A Basis for Greener Processes and Products, a.k.a., The “Shonan Guidance Principles,’ available at: [https://www.lifecycleinitiative.org/wp-content/uploads/2012/12/2011%20-%20Global%20Guidance%20Principles.pdf](https://www.lifecycleinitiative.org/wp-content/uploads/2012/12/2011%20-%20Global%20Guidance%20Principles.pdf).

<br><br>

[**_Return to TOC_**](./00-sub-handbook-landing.md)

