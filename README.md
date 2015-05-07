#ag-data-grid
**Experimental Work**
**For Polymer 0.5 Only.**
**Polymer 0.8 version coming later with breaking changes and more features!**

**ag-data-grid** is an Web Component to display tabular data.
It has built-in support for paging, search, filters, sortable columns and custom cell renderer.

ag-data-grid is responsive and can automatically hide columns on smaller screens based
on a few simple attributes defined by developer such as "importance" of a particular column.

##Demo
[Contacts List Grid Demo](https://aghassemi.github.io/webcomponents/ag-data-grid/demo.html)

##Install
```
bower install aghassemi/ag-data-grid
```
##Usage

Please see full API documentation on the [Component Page](https://aghassemi.github.io/webcomponents/ag-data-grid/).
###Basic
```
  <ag-data-grid summary="Displays each person's score"
    pageSize=5
    dataSource="{{dataSource}}">
    <ag-data-grid-column label="Name">
      <template>
        {{item.name}}
      </template>
    </ag-data-grid-column>
    <ag-data-grid-column label="Score">
      <template>
        {{item.score}}
       </template>
    </ag-data-grid-column>
  </ag-data-grid>
```
DataSource attribute expects an object that has a ```fetch(search, sort, filters)``` method.
Please see documentation on DataSource property for details.

###Full Featured
Please see ```demo.html``` for a full featured example.

##License
MIT