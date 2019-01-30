> Written with [StackEdit](https://stackedit.io/)
> 
## **XML File Format**
##*eXtensible Markup Language*
---------
> ####**Key Characteristics, History and Uses of XML File Format**

```xml
<?xml version=”1.0” encoding=”UTF-8”?>
	<note>
		<to>Tovee</to>
			<from>Jani</from>
		<heading>Reminder</heading>
	<body>Don't forget me this weekend!</body>
</note>
```
[2]:##### **Figure 1** *A sample of data in XML format* (Alhashami, Z., 2015)
> 
> Another example of text-based format, **XML** contrasts to plain text and binary formats with its increased complexity and comprehensibility – XML has the distinction of being self-describing, _in other words, being readable by both computers and humans._

>This is achieved by the labelling employed element and attribute for which each value is assigned. This can be seen in **[figure 1][2]**; the lines of metadata are accountable at the top of the dataset, followed by the matrix of values, each preceded by a descriptive label (also note the indenting. 

>The presence of _tags_ associated with values allows the human user to identify and locate values with the data and is scripted in language able to be directly readable by the computer.

>Hierarchical organisation is facilitated by _nesting_ capabilities inherent in the labeled elements and attributes to which the values are connected.

>This added organisation comes with the caveat that the choice of what is to be measured needs to be well thought out:
#### _The measurements of a dataset will need to fit into the existing organisation of the attributes of elements._
>In order for XML format data to be shared, the creator will specify a design for how it is to be read. This is known as a *schema* and is implemented using a language, in the case supplied in [Introduction to Data Technologies][1] it is the Document Type Data (DTD). 

>Established schema exist to act as frameworks for data in various fields, one such example is the “Essential Annotation Schema for Ecology” ([Pfaff, et al., 2017][2]) .  This framework works toward the goal of increasing data accessibility within the field of ecology

>As with other plain text formats, XML does not require any special software to be viewed, Microsoft Notepad or Mac TextEdit will suffice. The ability to easily share data in XML format is another benefit and can be done so, the main purpose of the XML format can be described in its ability to store, transport and structure data.

>  
[1]:https://www.stat.auckland.ac.nz/~paul/ItDT/HTML/node38.html#SECTION00925000000000000000)
[2]:https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5638456/
Alhashami, Z. (2015). XML Files Types and Their Differences and Denominators with Plain TXT File. Journal of Theoretical and Computational Science,02(03). doi:10.4172/2376-130x.1000130




