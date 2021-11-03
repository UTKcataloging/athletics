# Open Refine Template University of Tennessee Lady Volunteers Swimming and Diving


## Template

#### Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```
####Body

```
<mods>
<identifier type="local">{{cells["identifier"].value}}</identifier>

{{if(isBlank(cells['Eidentifier'].value), '', '<identifier type="pan">' + cells["Eidentifier"].value + '</identifier>')}}

{{if(isBlank(cells['title'].value), '', '<titleInfo><title>' + cells["title"].value + '</title></titleInfo>')}} 

<titleInfo supplied="yes"><title>{{cells['title_supplied'].value}}</title></titleInfo>

{{if(isBlank(cells['date_text'].value), '', '<originInfo><dateIssued>' + cells['date_text'].value + '</dateIssued><dateIssued encoding="edtf" keyDate="yes">' + cells['date_text'].value + '</dateIssued><publisher>' + cells['creator'].value + '</publisher><place><placeTerm valueURI="http://id.loc.gov/authorities/names/n79109786">Knoxville (Tenn.)</placeTerm>
</place></originInfo>')}}

<abstract>{{cells["abstract"].value}}</abstract>

<physicalDescription><form authority="aat" valueURI="{{cells['form_URI'].value}}">{{cells['form'].value}}</form><form authority="aat" valueURI="{{cells['form2_URI'].value}}">{{cells['form2'].value}}</form><extent>{{cells["extent"].value}}</extent></physicalDescription>

{{if(isBlank(cells['subject_topic'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_URI'].value + '"><topic>' + cells['subject_topic'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_topic_2'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_2_URI'].value + '"><topic>' + cells['subject_topic_2'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_topic_3'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_3_URI'].value + '"><topic>' + cells['subject_topic_3'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_topic_4'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_4_URI'].value + '"><topic>' + cells['subject_topic_4'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_topic_5'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_5_URI'].value + '"><topic>' + cells['subject_topic_5'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_topic_6'].value), '', '<subject authority="lcsh" valueURI="' + cells['subject_topic_6_URI'].value + '"><topic>' + cells['subject_topic_6'].value + '</topic></subject>')}}

{{if(isBlank(cells['subject_name'].value), '', '<subject authority="wikidata" valueURI="' + cells['subject_name_URI'].value + '"><name><namePart>' + cells['subject_name'].value + '</namePart></name></subject>')}}

{{if(isBlank(cells['subject_name_2'].value), '', '<subject authority="naf" valueURI="' + cells['subject_name_2_URI'].value + '"><name><namePart>' + cells['subject_name_2'].value + '</namePart></name></subject>')}}

{{if(isBlank(cells['subject_name_3'].value), '', '<subject authority="wikidata" valueURI="' + cells['subject_name_3_URI'].value + '"><name><namePart>' + cells['subject_name_3'].value + '</namePart></name></subject>')}}

<subject authority="naf" valueURI="{{cells['subject_geographic_URI'].value}}"><geographic>{{cells['subject_geographic'].value}}</geographic><cartographics><coordinates>{{cells['coordinates'].value}}</coordinates></cartographics></subject>

<typeOfResource>text</typeOfResource>

<relatedItem displayLabel="Project" type="host"><titleInfo><title>University of Tennessee Lady Volunteers Swimming and Diving Guides</title></titleInfo></relatedItem>

<location><physicalLocation valueURI="http://id.loc.gov/authorities/names/no2014027633">University of Tennessee, Knoxville. Special Collections</physicalLocation></location>

<recordInfo><recordContentSource valueURI="http://id.loc.gov/authorities/names/n87808088">University of Tennessee, Knoxville. Libraries</recordContentSource></recordInfo>

<accessCondition type="use and reproduction" xlink:href="{{cells['rights_URI'].value}}">{{cells['rights'].value}}</accessCondition>
</mods>

```

#### Suffix

```
</modsCollection>
```