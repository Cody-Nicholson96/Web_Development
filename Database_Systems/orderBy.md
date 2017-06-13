# ORDER BY

Select thing From list Where (Name = 'Hellen') ORDER BY (ordering attributes)

Tuples are sorted by the first attribute in the list

Ascending order is the default, DESC after attribute indicates descending order instead

Ties are broken by the second attribute (if any), then the third attribute (if any), et cetera

Example:

> Select student From studentTable Where (Program = 'COMP-SCI') ORDER BY lastName, firstName;
This example will display all of the rows that have the value 'COMP-SCI' in the Program column, and those rows will be sorted first by lastName, and next by firstName
