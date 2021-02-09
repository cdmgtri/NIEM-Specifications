---
  feedbackDate: DATE
---

This is a landing page for information about the set of NIEM specifications, managed by the NIEM Technical Architecture Committee (NTAC).

- TOC
{:toc}

## Announcements

<div markdown="1" class="note">

The following NIEM specifications have drafts ready for review, with feedback requested by {{ page.feedbackDate }}.

{% assign drafts = site.data.specifications | where: "status", "draft" %}

{% for draft in drafts %}

  {% assign class = site.data.classes | where: "id", draft.classID | first %}

- **[{{ class.name }}]({{ draft.url }}), Version {{ draft.version }}**
  <br/>Published {{ draft.year }}. See [changes]({{ draft.changeHistory }}). Submit feedback [here]({{ class.repo | append: "/issues/new" }}).

{% endfor %}

</div>

## NIEM Naming and Design Rules (NDR) Specification

{% include section.html classID="NDR" %}

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

{% include section.html classID="IEPD" %}

## NIEM JSON Specification

{% include section.html classID="JSON" %}

## NIEM Code Lists Specification

{% include section.html classID="CodeLists" %}

## NIEM Conformance Specification

{% include section.html classID="Conformance" %}

## NIEM Conformance Targets Attribute Specification (CTAS)

{% include section.html classID="CTAS" %}

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
