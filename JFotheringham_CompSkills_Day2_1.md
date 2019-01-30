> Written with [StackEdit](https://stackedit.io/).
## **Plain Text Format**
## *CSV Delimited*
----------
> ####**Key Characteristics, History and Uses of CSV Delimited File Format**
000,VERSIONS:,1:8.4a3,1:8.3.3,1:8.2.3,1:8.1.1,1:8.0.5
001,CATCH return ok,11,6,7,4,5
002,CATH return error,70,64,275,54,204
003,CATCH no catch used,10,6,7,13,4
004,IF if true numeric,17,11,13,7,9
005,IF elseif true numeric,20,15,16,20,11
#####__becomes:__
 >|000|VERSIONS:|1:8.4a3|1:8.3.3|1:8.2.3|1:8.1.1|1:8.0.5|
|----|----|----|----|----|----|----|
| 001 | CATCH return ok | 11 | 6 | 7 | 4 | 5 |
| 002 | CATH return error | 70 | 64 | 275 | 54 | 204 |
| 003 | CATCH no catch used | 10 | 6 | 7 | 13 | 4 |
| 004 | IF if true numeric | 17 | 11 | 13 | 7 | 9 |
| 005 | IF elseif true numeric | 20 | 15 | 16 | 20 | 11 |
##### **Figure 1**  *A sample of data in plain text CSV format*

>CSV format falls under the umbrella of plain text formats, the most simplistic of data storage formats.
The data is stored as a sequence of characters, which are stored in the memory as a series of bytes (8 bit units), each character made up of one or two bytes.

>Various coding systems can be employed to handle plain text formatted data, most commonly in US English, the ASCII (American Standard Code for Information Interchange)

>The file can be delimited or fixed width and data is organised into rows, with the values of the attributes or … on each row and depending on the nature of file either separated by a delimiter (or in the case of a CSV file, a comma) , or by the predetermined number of characters allocated to a row.

>Navigating and searching for data in a plain text formatted file can be cumbersome as the file does not specify identifying articles like whether the value is a number or text, or a reference of where the data value is. However, the simplicity of this format makes it almost universal and accessible to most software and different platforms, it is high on the interoperability scale.
 
> For this reason it remains a commonly used format throughout Earth Science/Ecology fields – it is the simplest way to store information and can be relied upon to perform under the conditions it was designed.
It is known as the oldest form of data organisation and pre-dates computers, and is claimed to be the most commonly used file format and recommended in guidelines for data management standards. [British Ecology Society][1]

> CSV can be handled in spreadsheet and statistical computing software; Microsoft Excel and Rstudio/Matlab amongst others.
> 
> [Introduction to Data Technologies](https://www.stat.auckland.ac.nz/~paul/ItDT/HTML/node38.html#SECTION00925000000000000000)

[1]:(https://www.britishecologicalsociety.org/wp-content/uploads/Publ_Data-Management-Booklet.pdf)



