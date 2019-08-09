## TIPNR - Tyndale Individualised Proper Names with all References - TyndaleHouse.com STEPBible.org CC BY-NC   
Proper Nouns in the ESV (+ differences in KJV & NIV) with unique tag for each individual and location, with Hebrew/Greek forms and an exhaustive list of occurences  

Data created for www.STEPBible.org by Tyndale House Cambridge (CC BY-NC 4.0)  
_Modified by Robert Rouse to tranform into JSON format_

This licence allows you to:
* Include any part of this data in free software or free publications without requesting permission 
* Request permission if your project is not free. A reasonable request is unlikely to be refused.
* Download the data and reformat it for your application
* Refer others to this repository as the source of the data.
And you should:
* List any changes you make to the data. Please also send changes to TyndaleStep@gmail.com so that others can benefit.
* Attribute the original data to "Tyndale House, Cambridge" linked to www.TyndaleHouse.com, 
  and to "STEP Bible" linked to www.STEPBible.org
* Link to its source at https://tyndale.github.io/STEPBible-Data/

If you use this data, we'd love to hear about your project when you make it available. Email us at TyndaleSTEP@Gmail.com.
___



## FIELD DESCRIPTIONS:

Header fields for  Individuals: 
* Unique name - made up of the most common English form of the name + the 1st instance where that person/place occurs, 
  - e.g. Abraham@Gen.11.26. Note that at Gen.11.26 he is actually called Abram, but the unique name is based on the most common form.
* Description - very basic such as "Place" or "Male living at the time of the first Patriarchs"
 - they will become: Name (aka aliases), Significance, Date, Son of, Married to, Descended from; where Date is the century except "2nd M BC" for Abraham to Saul, "3rd M BC" for Noah to Terah, and "before the 3rd M BC" for anything before Noah. 
* Parents - the Unique names in the form of Father + Mother, e.g. "Terah@Gen.11.24 + " (because the mother is unknown)
* Siblings - the Unique names separated by commas
* Partners - the Unique names  of the husband or wife/wives 
* Offspring - the Unique names of any children

Header fields for Places:
* Unique name (as for Individuals)
* OpenBible name - i.e. the name used at http://www.openbible.info/geo/
* Geoposition - as defined by OpenBible

Fields in linked subRecords (i.e. one line for every Greek+Hebrew form of the name of that individual/place or the same Greek/Hebrew but with different translations): 
* UniqueTag which is usually identical to the UniqueName though if the translation is different it is prefaced with "|"  - e.g. "Abram|Abraham@Gen.11.26"
* Hebrew or Greek form of the name with Strong number, augmented with letters to line it up with the larger dataset in BDB  - e.g. H6152a="Arabia" and H6152b="west" but sometimes translated "Arabia". Variant for OT ("Ketive" & "Qere") and NT ("Var.") differences are recorded only where they make a difference to the translation of the name.
* translation in ESV (with alternates in NIV & KJV when they are different - not exhaustive).
* exhaustive list of all refs where this form of the Hebrew or Greek  occurs in the OT or NT respectively using Standard English versification

Each record starts with "$" and fields are separated by Tabs. 
The first line is a Header, and subsequent lines are linked subRecords which all start with a tab (i.e. an emty field). The fields in the Header can be regarded as the initial fields for each linked subRecord. 
The fields in Headers for individuals and places are different:

$========== PERSON(s)
UniqueName	Description	Parents Male+Female	Siblings	Partners	Offspring
	UniqueTag	Hebrew/Greek	ESV name	Refs

$========== PLACE
UniqueName	Description	OpenBible name	Geoposition at OpenBible
	UniqueTag	Hebrew/Greek	ESV name	Refs

$========== OTHER
UniqueName	Description	
	UniqueTag	Hebrew/Greek	ESV name	Refs

So, for a place name, the fields in the Header line are: Unique name, Description, OpenBible name, and Geoposition at OpenBible. These fields apply to each of the following linked subRecords which each contain the additional fields: UniqueTag, Heberew/Greek form, ESV Translation (with differences in KJV or NIV) and an exhaustive list of refences where this form and translation occurs. 
For an individual the fields in the linked subRecords are identical, but the Header line contains the fields: Description, Parents, Siblings, Partners and a list of Offspring.
When there is uncertainty about whether someone or some place in one reference is identical to the same name used in another place, this dataset tends to create a separate entry, unless there are good reasons to believe that they are identical. 
 
