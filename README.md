# Ext.ux.Exporter

## About

Exporter is a generic export class which takes any Ext.data.Store-based component (e.g. grids and similar) and exports the data in any format.

Exporter works completely client-side.  It uses a Formatter class to generate a document (.xls, .csv etc) and then uses the donwloadify library so that the user can view or download it.

Right now, there isn't a readme or example. You can check this post for more info for now: http://www.sencha.com/forum/showthread.php?136598-Export-store-to-Excel

# More details provided by Mason Zhang
## How to use it
- include script files in html file:
```
    <script type="text/javascript" src="/extjs/src/ux/exporter/swfobject.js"></script>

    <script type="text/javascript" src="/extjs/src/ux/exporter/downloadify.min.js"></script>
```
- in your items list, add an item as follows:
```
    {
        xtype: 'exporterbutton'
    }
```

## Notes
- currently I just make csv works
- the output excel file still does not work, excel has some errors when parse the xml format.