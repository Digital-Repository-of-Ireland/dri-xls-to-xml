# dri-xls-to-xml

## Requirements
 * Windows OS
 * Microsoft Excel

## Install
To install, save the add-in, then in Excel, go to the Developer tab (https://msdn.microsoft.com/en-us/library/bb608625.aspx) , and select Add-Ins, and then Browse. Find where you saved the add-in file and select it. Once installed this should create a new tab 'Add-Ins' after Developer, with one option 'DRI XML Export'.

The spreadsheet column headings should correspond to the elements that you wish to appear in the XML file, e.g., dc:title, dcterms:spatial. There also needs to be an 'Output file' column that gives the filename that the generated XML will be saved to. If you want to change the output location you should be able to append a folder to the values in the output file column.

## Example
An example spreadsheet could have the following column headings:

dc:title | dc:description | dc:creator | dc:date xsi:type="dcterms:W3CDTF"| dc:type xsi:type="dcterms:DCMIType" | dc:rights | Output File
---------|----------------|------------|----------------------------------|-------------------------------------|-----------|------------
An Object | Description of the object | A. N. Other | 2019-05-14 | Text | A rights statement | object1.xml
