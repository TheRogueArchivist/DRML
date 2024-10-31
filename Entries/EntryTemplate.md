# Entry Information:

{Entry template to help standardize the style and contents of DRML entries. All text within curly brackets should be removed or replaced with the relevant information, even if that information is simply "N/A", "Unknown", or an equivalent. Section names or other text not in curly brackets should be considered standard and shouldn't be removed. If changes are needed, they should be generalized to work with all existing entries, and this template should be edited to reflect that.}

## DRML Entry Name:

**{Entry name}**

***

## Authors/Contributors:

* {Unordered list containing entry authors and major contributors.}

***

## Table of Contents:

{This curly-bracket enclosed block of text should be removed in the final entry. The table of contents links to sections within the entry. The format is `[Header Name](#header-name)`, where the portion in parentheses is ``"#" + "name of the header in all lowercase with spaces replaced with a dash"``. If there are two words, also add a second link next to the first one with the format of `[Alt.](#Header%20Name)`, where the portion in parentheses is ``"#" + "name of the header (with original case preserved) with spaces replaced with %20"``. This is to maintain compatibility with Markdown readers (such as Obsidian) that don't recognize the first way to link to internal sections in a document.}

* [Entry Information](#entry-information) ([Alt.](#Entry%20Information))
	* [DRML Entry Name](#drml-entry-name) ([Alt.](#DRML%20Entry%20Name))
	* [Authors/Contributors](#authors/contributors)
	* [Table of Contents](#table-of-contents) ([Alt.](#Table%20of%20Contents))
	* [Categories](#categories)
	* [Software Known to Detect](#software-known-to-detect) ([Alt.](#Software%20Known%20to%20Detect))
	* [Preservation Instructions](#preservation-instructions) ([Alt.](#Preservation%20Instructions))
* [DRM Information](#drm-information) ([Alt.](#DRM%20Information))
	* [Names](#names)
	* [Developers](#developers)
	* [Protection Features](#protection-features) ([Alt.](#Protection%20Features))
	* [Overall Description](#overall-description) ([Alt.](#Overall%20Description))
	* [Timeline](#timeline)
		* {Series of level 4 headers to split up timeline into manageable chunks.}
	* [Versions & Differences](#versions-&-differences) ([Alt.](#Versions%20&%20Differences))
		* [Tested](#tested)
		* [Untested](#untested)
	* [Samples](#samples)
		* [Confirmed](#confirmed)
		* [Unconfirmed](#unconfirmed)
	* [Supported Platforms](#supported-platforms) ([Alt.](#Supported%20Platforms))
	* [Associated File Attributes](#associated-file-attributes) ([Alt.](#Associated%20File%20Attributes))
		* {Series of level 3 headers used to denote what attribute this entry's DRM has which can be used to identify it. TODO: Make standard list of file attributes that may be used.}
			* {Level 4 headers under each level 3 header in this section used to list the identifying content of the file attribute of this entry's DRM.}
* [Reference Material](#reference-material) ([Alt.](#Reference%20Material))
	* [Media](#media)
	* [Additional Resources](#additional-resources) ([Alt.](#Additional%20Resources))
		* {Series of level 3 headers used to organize the various resources as effectively as possible.}
	* [Footnotes](#footnotes)

*** 

## Categories: 

* {Unordered list of applicable categories. TODO: Add list of categories here.}

***

## Protection Features:

* {Unordered list of applicable protection features. TODO: Add list of protection features here.}

***

## Software Known to Detect:

* {Unordered list of software able to detect DRM. TODO: Add list of most common programs here.}

***

## Preservation Instructions:

{Instructions for how to effectively preserve media or content with this entry's DRM, including how to properly dump media and use content protected by it}

*** 

# DRM Information:

## Names: 

* {Unordered list of names that this entry's DRM is known to go by. This can include official and unofficial names, including names coined by the DRML entry itself. Every name must have a footnote that either cites where it comes from, or explains why the name has been coined.}

***


## Developers:

* {Unordered list of developers and/or publishers of this entry's DRM. This will usually be the company's name, but can be a person's name when especially relevant.}

***

## Overall Description:

{Freeform space for notes and discussion about this entry's DRM.}

***

## Timeline: 

#### {Series of level 4 headers to split up timeline into manageable chunks.}
* {Unordered list of specific events that occur within the time period specified by the level 4 header the list is under.}

***

## Versions & Differences: 

#### Tested:

* {Unordered list of tested versions. Should include name of product if applicable and version number, in whatever format makes most sense for the naming and versioning of this entry's DRM.}

#### Untested:

* {Unordered list of untested versions. Should include name of product if applicable and version number, in whatever format makes most sense for the naming and versioning of this entry's DRM.}

***

## Samples:
 
#### Confirmed:

* {Unordered list of *personally* confirmed samples of this entry's DRM. This may include any form of media or content protected. Footnotes must be added to indicate the exact copy of the media or content the DRM has been found in. Links to actual copies of the media or content are strongly preferred, so that readers may investigate the DRM themselves as easily as possible. If this isn't possible, the most identifying and specific source should be provided, such as a Redump entry for a game as that contains the hash.}

#### Unconfirmed: 

* {Unordered list of media or content that may contain samples of this entry's DRM. The reason why it's suspected to contain the DRM should be added in a footnote. If any specific copies or versions of the media or content have been investigated and found to not contain it, those should be added in a footnote as well.}

***

## Supported Platforms:

* {Unordered list of platforms this entry's DRM is supported on. This should include specific versions or products, if known.}

***

## Associated File Attributes:

### {Series of level 3 headers used to denote what attribute this entry's DRM has which can be used to identify it. TODO: Make standard list of file attributes that may be used.}

#### {Level 4 headers under each level 3 header in this section used to list the identifying content of the file attribute of this entry's DRM.}
{Further elaboration of the content, such as which files, products, versions, etc., it's found in, or what this content is known to do. For example, if file names are being listed, then this should specify what the files do if known.}

***

# Reference Material:

## Media: 

{This section is intended for media which can be collected from this entry's DRM, such as screenshots. Media either directly included in the DRM (such as splashscreen files themselves) or provided by outside sources (whether official or unofficial) should be linked to separately in the "Additional Resources" section. This section is currently only made to support images, though other media may possibly in scope with the proper adjustments to the template.}

1. {Ordered list, where each item is given a brief description before being directly embedded into the entry. The actual embedded media should be described as thoroughly as possible for accessibility. TODO: Add example image to template.}

***

## Additional Resources:

### {Series of level 3 headers used to organize the various resources as effectively as possible.}

{Further context to these resources may be given here, if needed.}

* {Unordered list of URLs. All should be links to the archived page if possible, to prevent link rot and ensure relevant information isn't changed. The link description should be an accurate description of the link, followed by relevant information in parentheses or square brackets. Use square brackets for most miscellaneous, such as language used. Use parentheses to specify a date, which should be in the ISO 8601 standard and prefaced by what the date represents. For example, if a link is archived, add "(Archived XXXX-YY-ZZ)" to the end of the link description.}

***

### Footnotes:

{This section should be completely empty in the editor. This section will be automatically populated by the footnotes created throughout the document, which should be created at the end of the section they are first used in. Names for each footnote should be sufficiently descriptive to clearly indicate what footnote they're referring to in the document to avoid confusion. These names don't need to be overly descriptive, but it's better to err on the side of being too descriptive instead of not descriptive enough.}
