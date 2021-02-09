---
  feedbackDate: DATE
  drafts:
    - id: IEPD
      name: Information Exchange Package Documentation (IEPD) Specification
      draft: Version 5.0 beta1
      published: February 2021
      url: https://niem.github.io/MPD-Spec/draft/niem-iepd-spec.html
      changes: https://github.com/NIEM/MPD-Spec/releases/tag/v5.0beta1
      feedback: https://github.com/NIEM/MPD-Spec/issues/new

    - id: Conformance
      name: Conformance Specification
      draft: Version 5.0 beta1
      published: December 2020
      url: https://niem.github.io/NIEM-Conformance-Spec/draft/niem-conformance-spec.html
      changes: https://github.com/NIEM/NIEM-Conformance-Spec/releases/tag/v5.0beta1
      feedback: https://github.com/NIEM/NIEM-Conformance-Spec/issues/new
---

This is a landing page for information about the set of NIEM specifications, managed by the NIEM Technical Architecture Committee (NTAC).

- TOC
{:toc}

## Announcements

<div markdown="1" class="note">

The following NIEM specifications have drafts ready for review, with feedback requested by {{ page.feedbackDate }}.

{% for spec in page.drafts %}
- **[{{ spec.name }}]({{ spec.url }})**, **{{ spec.draft }}**
  <br/>Published {{ spec.published }}. See [changes]({{ spec.changes }}). Submit feedback [here]({{ spec.feedback }}).

{% endfor %}

</div>

## NIEM Naming and Design Rules (NDR)

The [NIEM Naming and Design Rules (NDR) Specification](https://niem.github.io/NIEM-NDR/) describe the architecture of the NIEM data model and its representation in XML. It specifies principles and enforceable rules for NIEM data components and schemas.  Read more about the NDR on [niem.github.io](https://niem.github.io/reference/specifications/ndr/).

Submit a [new issue](https://github.com/NIEM/NIEM-NDR/issues/new), view [all issues](https://github.com/NIEM/NIEM-NDR/issues), track [issue status](https://github.com/NIEM/NIEM-NDR/projects/1), or go to the [GitHub repo](https://github.com/NIEM/NIEM-NDR) for this specification.

**Available versions**

- **[Version 5.0](https://niem.github.io/NIEM-NDR/v5.0/niem-ndr.html)**, published December 2020 - **[current version]**.  See [changes](https://github.com/NIEM/NIEM-NDR/releases/tag/v5.0).
- **[Version 4.0](https://reference.niem.gov/niem/specification/naming-and-design-rules/4.0/niem-ndr-4.0.html)**, published 2017
- **[Version 3.0](https://reference.niem.gov/niem/specification/naming-and-design-rules/3.0/niem-ndr-3.0.html)**, published 2014
- **[Version 1.3](https://reference.niem.gov/niem/specification/naming-and-design-rules/1.3/niem-ndr-1.3.pdf)**, published 2008

<details>
<summary markdown="span">Expand for Schematron rule bundles and more NDR resources...</summary>

<div markdown="1">

> The [Conformance Testing Assistant (ConTesA)](https://tools.niem.gov/contesa/) is an online tool that offers NDR conformance validation testing for NIEM XML schemas.  Conformance validation can also be tested locally with the NDR Schematron rules provided here.  Download a zip file below and see the [instructions](https://niem.github.io/reference/specifications/ndr/oxygen-schematron/) on how to test NDR conformance using the Oxygen XML Editor.
>
> - [NDR 5.0 resources](https://niem.github.io/NIEM-NDR/v5.0/niem-ndr-v5.0.zip)
> - [NDR 4.0 resources](https://reference.niem.gov/niem/specification/naming-and-design-rules/4.0/niem-ndr-4.0.zip)
> - [NDR 3.0 resources](https://reference.niem.gov/niem/specification/naming-and-design-rules/3.0/niem-ndr-3.0.zip)
</div>

</details>

## NIEM Information Exchange Package Documentation (IEPD) Specification

The NIEM Model Package Description (MPD) Specification specifies normative rules and non-normative guidance for building NIEM information exchange messages. It defines IEPD artifacts like subset schemas, extension schemas, and MPD catalogs; and recommends how the package should be structured.

> Note: This specification was formerly known as the **NIEM Model Package Description (MPD) Specification**.

Submit a [new issue](https://github.com/NIEM/MPD-Spec/issues/new), view [all issues](https://github.com/NIEM/MPD-Spec/issues), or go to the [GitHub repo](https://github.com/NIEM/MPD-Spec) for this specification.

**Available versions**

{% assign spec = page.drafts | where: "id", "IEPD" | first %}

- **[IEPD {{ spec.draft }}]({{ spec.url }})**, published {{ spec.published }} - **[latest draft]**.  See [changes]({{ spec.changes }}).
- **[MPD Version 3.0.1](https://niem.github.io/MPD-Spec/v3.0.1/model-package-description-3.0.1.html)**, published 2015.

## NIEM JSON Specification

The NIEM JSON Specification establishes the technical basis for using JavaScript Object Notation (JSON) as a data format for exchange of information consistent with NIEM-conformant schemas and message specifications.

Submit a [new issue](https://github.com/NIEM/NIEM-JSON-Spec/issues/new), view [all issues](https://github.com/NIEM/NIEM-JSON-Spec/issues), track [issue status](https://github.com/NIEM/NIEM-JSON-Spec/projects/1), or go to the [GitHub repo](https://github.com/NIEM/NIEM-JSON-Spec) for this specification.

**Available versions**

- **[Version 4.0](https://niem.github.io/NIEM-JSON-Spec/v4.0/niem-json-spec.html)**, published 2020 - **[current version]**

## NIEM Code Lists Specification

The NIEM Code Lists Specification adds support for new capabilities of NIEM code lists beyond the basic enumeration representations provided by XML and JSON schema (simple sets of fixed-schema code values and definitions). Key new features include the definition of codes in CSV or Genericode files, dynamic code lists via run-time binding, and multi-column code table support.

Submit a [new issue](https://github.com/NIEM/NIEM-Code-Lists-Spec/issues/new), view [all issues](https://github.com/NIEM/NIEM-Code-Lists-Spec/issues), track [issue status](https://github.com/NIEM/NIEM-Code-Lists-Spec/projects/1), or go to the [GitHub repo](https://github.com/NIEM/NIEM-Code-Lists-Spec) for this specification.

**Available versions**

- **[Version 4.0](https://reference.niem.gov/niem/specification/code-lists/4.0/niem-code-lists-4.0.html)**, published 2020 - **[current version]**

## NIEM Conformance Specification

The [NIEM Conformance Specification](https://niem.github.io/NIEM-Conformance-Spec/) introduces the idea of NIEM conformance and provides a general normative definition for its meaning, how it applies, and to what it does and does not apply. It describes the benefits of conformance, and refers to sources of information, tools, and help. Read more about it on [niem.github.io](https://niem.github.io/reference/specifications/conformance/).

Submit a [new issue](https://github.com/NIEM/NIEM-Conformance-Spec/issues/new), view [all issues](https://github.com/NIEM/NIEM-Conformance-Spec/issues), or go to the [GitHub repo](https://github.com/NIEM/NIEM-Conformance-Spec) for this specification.

**Available versions**

{% assign spec = page.drafts | where: "id", "Conformance" | first %}

- **[{{ spec.draft }}]({{ spec.url }})**, published {{ spec.published }} - **[latest draft]**.  See [changes]({{ spec.changes }}).
- **[Version 3.0](https://reference.niem.gov/niem/specification/conformance/3.0/conformance-3.0.html)**, published 2014 - **[current version]**
- **[Version 1.0](https://reference.niem.gov/niem/specification/conformance/1.0/conformance-1.0.pdf)**, published 2008

<style>
.note {
  background: rgba(255, 239, 213, 0.5);
  border: solid 1px blanchedalmond;
  border-radius: 4px;
  font-size: 15px;
  margin: 0 0 20px;
  padding: 10px 20px;
}
</style>
