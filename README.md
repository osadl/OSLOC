# Open Source License Obligations Checklists
The official project website is [https://www.osadl.org/OSLOC](https://www.osadl.org/OSLOC).
## Background and goal of the project
Whenever Open Source software is copied and distributed which typically is permitted by every type of Open Source license, a number of obligations and prohibitions are imposed on the distributor. It is very common for the recipients of such software to recursively redistribute it in such a way that a chain of distributors and recipients is created &ndash; all of them having to fulfill the same license obligations. This project aims to establish a common understanding of how these obligations are to be fulfilled that is accepted by distributors and copyright holders and trusted by all members of the distribution chain.

In order to be accepted by a large variety of professionals, the checklists must be written in plain English language using the identical words for the same condition or action. However, in many cases different license texts use different words for the same condition or action which makes it necessary to create a vocabulary of common license terms. This vocabulary must clearly describe every item of the vocabulary in such a way that it can be used to create canonical versions of the license texts. Using this vocabulary, a selection of frequently employed and important Open Source licenses is compiled into checklists.
## Access
The recommendations given by the license obligations checklists are not made to be taken as individual legal advice, which in some countries, in particular Germany, can only be given by certified personnel, i.e. lawyers. Therefore, access to the project material can be gained in two ways:
1. Access to the interactive user interface where use cases can be chosen to create customized checklists is granted on request. Please contact OSADL at info@osadl.org to receive login data, information on the project and the legal disclaimer.
2. However, the raw data from which the checklists are created are available without access restrictions. This material may be incorporated into scanning tools, companies' internal utilities, and similar tools. Consequently, it is then the users' own responsibility to supply the checklist information in compliance with the national rules on legal advice. These raw data are available in this repository or along with some examples of how to use them at [https://www.osadl.org/RawChecklists](https://www.osadl.org/RawChecklists).
## The checklists
### "Language" elements, "Actions" and "Terms"
On the base level, a license contains obligations (“YOU MUST”) and prohibitions (“YOU MUST NOT”). In order to allow for the extraction of license obligation and prohibition in atomic granularity, “YOU MUST” and “YOU MUST NOT” atoms may be repeated as often as required. The atoms are understood as logical “and” elements, i.e. all of them must be followed to reach license compliance. The arguments of the atoms, i.e. what must or what must not be done, are described with words that are selected from a vocabulary of actions and terms which are defined by a distinct description of each item.

Sometimes the license obligation atoms may allow the distributor to freely select between a number of optional use cases; therefore, the “USE CASE” element is introduced which, in turn, may again be followed by “YOU MUST” and “YOU MUST NOT” atoms depending on the selected option. Several "USE CASE" elements to which the same license conditions apply may be combined using the "OR" element. In addition, the license may contain certain obligations that are only applicable in case a particular unalterable condition is present; to encode such a situation the “YOU MUST” and “YOU MUST NOT” atoms may be preceded by the “IF” element along with a condition. To further specify a term, it may be followed repeatedly by an “ATTRIBUTE”. Finally, elements may be negated by preceding it with the element "NOT".
### Hints to compatibility, patents and copyleft
If a license has a copyleft clause, it is marked and referenced using the "COPYLEFT CLAUSE" language construct. The same applies to patent hints which are encoded using the "PATENT HINTS" language construct. Compatibility with another license, i.e. whether software that uses another license can be integrated into software that uses the current license and copied and distributed in a compliant way is encoded and referenced using the "COMPATIBILITY" language construct. Incompatibility is encoded in a similar way, but there is an exception how referencing is handled, since two references separated by a vertical bar are required after the "INCOMPATIBILITY" language construct &ndash; the first one is the license obligation of the other license and the second one is the contradicted license obligation of the current license. Non-copyleft licenses are implicitly assumed to be compatible between each other.

The compatibility of all licenses with each other is given as a matrix in the directory [compatibility-matrix](https://github.com/osadl/OSSLCC/tree/master/compatibility-matrix). In raw data form, this information is available in JSON format as a nested array with the outer array containing the leading licenses (i.e. the rows of the matrix) and the inner array containing the secondary licenses (i.e. the columns of the matrix). In addition, it comes in three variants:
* As an associative array
* As a sequentially indexed array
* As a sequentially indexed array with explanations
### Checklists
The license checklists along with references to the original license text are given in the directory [licenses](https://github.com/osadl/OSSLCC/tree/master/licenses). The license checklists without the reference are given in the directory [unreflicenses](https://github.com/osadl/OSSLCC/tree/master/unreflicenses).
## Licensing
Copyright (c) 2018-2022 Open Source Automation Development Lab (OSADL) eG  

Licensed under CC0-1.0.

To the extent possible under law, the person who associated CC0-1.0 with OSSLCC has waived all copyright and related or neighboring rights to OSSLCC.

For the original license text see [http://creativecommons.org/publicdomain/zero/1.0/](http://creativecommons.org/publicdomain/zero/1.0/).
