> Written with [StackEdit](https://stackedit.io/).
## **Rational Database File Format**
##*Rational Database*
---------
> ####**Key Characteristics, History and Uses of Rational Database File Format**

----------
These data storage file formats are considered conceptually complex and are typically facilitators of very large or very complex datasets.

Rational Databases are composed of tables and are somewhat differentiated from other formats by the defined structure in which they are designed.

>To view/store/edit databases, the user requires a **Database Management System** (DBMS).

Some of the particular powers of the database for data storage is in its ability to manipulate data by breaking up and reforming tables based on relational elements.

This is done with the assignment of *keys* to table entities flowpath; **primary keys** connect an object data and, therefor, tables with the **foreign key**.

>The assignment of  between keys in a simple one-to-one relationship can be described by the diagram;
```flow
st=>start: Primary Key Table 1
e=>end: Foreign Key Table 2
op=>operation: one-to-one Relationship
st->op->e
```
 
> Extending on this, cardinality of relationships linking tables can more complex:  one-to-many, where many tables relate to one, and many-to-many, where an attribute cannot be expressed as primary or foreign, but rather both, in this situation a new table is constructed to express this complex relationship.
 
The design of a database is concerned with the parameters of **how many** *tables* are included, how those tables are **linked** and **what information** is held and linked within those tables. These are defined by the choice of entities and attribute and ultimately guide the functionality of the database.

The three rules by which the design of a streamlined database is created are known at the first, second and third *“normal form”*.  The culmination of implementing these rules will result in a compact database, without repetition, thus increasing ease in alteration and reducing error.
>if each element is only entered once, making corrections to an piece of information will, in turn, also only need to be done once.

The complexity level inherent in relational databases enables their power to store and organise large volumes of data and allows for tailored organisational structures to be created to suit a host of needs. The trade-off for this power being the costs in the creation of a database, which is relatively high, and that specific software is required to access them. 


[Introduction to Data Technologies(2009)][1]
[1]:https://www.stat.auckland.ac.nz/~paul/ItDT/HTML/node38.html#
