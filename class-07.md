# HTML tables and JS constructor functions

## HTML tables

Tables are relatively easy to construct in HTML. THey can be initialized with the `<table>` tag. Each row is constructed with the `<tr>` element and each cell within each row with the `<td>` element, or add a heading cell with the `<th>` element. You can change whether the `<th>` heads a collumn or a row with the `scope` attribute which should be set to `col` or `row` respectively. You can have an element span multiple rows or collumns with the `rowspan` and `colspan` attributes, which should be set to integer values determining the number of rows/collumns to span. You can add specific tags to easily identify the first and last rows of the table with `<thead>` and `<tfoot>` respectively, and the body with the `<tbody>` element.

## JS constructors

Constructors are an alternate way to create objects other than object literals. You can make a new object by setting a new variable to `let exampleObj = new Object();`, and then properties and methods can be added like so: `exampleObj.exampleProperty = '[examplevalue]'`, or `exampleVar.exampleMethod = function(input) { return input + 5;}`, respectively. You can remove properties or methods with the `delete` tag, for instance `delete exampleObj.exampleKey;`.
