---
title: Overview
page_title: Overview
description: Overview
slug: gridview-events-overview
tags: overview
published: True
position: 0
---

# Overview


This topic covers the specific events exposed by the __RadGridView__ control and its sub elements __GridViewColumn__, __GridViewRow__ and __GridViewCell__. The events are first grouped by control and then by their general purpose.

## RadGridView


### Data Events
            

* __DataLoading__: Occurs before the grid view data is loaded. The type of the passed event arguments is __GridViewDataLoadingEventArgs__.
              

* __DataLoaded__: Occurs when the grid view data is loaded. The type of the passed event arguments is
{% if site.site_name == 'WPF' %}__System.EventArgs__{% endif %}{% if site.site_name == 'Silverlight' %}__GridViewDataLoadingEventArgs__.
{% endif %}

* __BindingValidationError__: Occurs when a data validation error is reported by a binding source. The type of the passed event arguments is __EventArgs__.
              

* __AddingNewDataItem__: Occurs when a new data item is about to be added. The type of the passed event arguments is __GridViewAddingNewEventArgs__.
              

### Selection Events
            

* __CurrentCellChanged__: Occurs when the selected grid cell has changed. The type of the passed event arguments is __GridViewCurrentCellChangedEventArgs__.
              

* __SelectionChanged__: Occurs when the selected grid row has changed. The type of the passed event arguments is __SelectionChangeEventArgs__.
              

* __RowActivated__: Occurs when a row is activated - when user double click on it or press enter. The type of the passed event arguments is __RowEventArgs__      


* __RowLoaded__: Occurs anytime the row appears within the view port. The type of the passed event arguments is __RowLoadedEventArgs__.
                

* __RowUnloaded__: Occurs anytime the row disappears within the view port. The type of the passed event arguments is __RowUnloadedEventArgs__.
                

### Edit Events 


* __RowEditEnded__: Occurs when row validation passed successfully and new data is committed to the __RadGridView__.__ItemsSource__. The type of the passed event arguments is __GridViewRowEditEndedEventArgs__.
            

* __CellEditEnded__: Occurs when cell validation is passed successfully and new data is committed to the __RadGridView__.__ItemsSource__. The type of the passed event arguments is __GridViewCellEditEndedEventArgs__.
            

* __BeginningEdit__: Occurs when the cell is about to enter into EditMode. The type of the passed event arguments is __GridViewBeginningEditRoutedEventArgs__.
            

* __PreparingCellForEdit__: Occurs after the BeginningEdit event. It allows you to obtain a reference to the editing element and change its properties.
            

* __PreparedCellForEdit__: Occurs after the PreparingCellForEdit event.

[Read more]({%slug gridview-events-edit%})            

### Delete Event 
[Read more]({%slug gridview-events-delete%})
          

### Validation Events 
[Read more]({%slug gridview-events-validation%})
        

### Filtering Events 
[Read more]({%slug gridview-filtering-basic%})
        

### Sorting Events 

        

* __Sorting__: Occurs when the grid data is about to be sorted. The type of the passed event arguments is __GridViewSortingEventArgs__.
          

* __Sorted__: Occurs when the grid data has been sorted. The type of the passed event arguments is __GridViewSortedEventArgs__.

[Read more]({%slug gridview-sorting-basics%})


### Grouping 
           

* __Grouping__: Occurs when the grid data is about to be grouped. The type of the passed event arguments is __GridViewGroupingEventArgs__.

* __Grouped__: Occurs when the grid data has been grouped. The type of the passed event arguments is __GridViewGroupedEventArgs__.

* __ChildTableDefinitionAdded__: Occurs when a new child table definition has been added. The type of the passed event arguments is __TableDefinitionCreatedEventArgs__.

[Read more]({%slug gridview-grouping-basics%})

### Exporting Events 
          
* __ElementExporting__: Occurs when the grid data is being exported. It is a direct replacement of the __Exporting__ event.
          

* __ElementExported__: Occurs after the __ElementExporting__ event where you can access the StreamWriter and write additional data to the stream.

* __ElementExportingToDocument__: Occurs when the grid data is being exported to Xlsx or Pdf.

* __ElementExportedToDocument__: Occurs after the ElementExportingToDocument event. Within it you can access the StreamWriter and write additional data to the stream.

[Read more]({%slug gridview-export-events%})          

### Row Details Events
        

* __UnloadingRowDetails__: Occurs when the row details are being unloaded. The type of the passed event arguments is __GridViewRowDetailsEventArgs__.
          

* __RowDetailsVisibilityChanged__: Occurs when the visibility of the row details has changed. The type of the passed event arguments is __GridViewRowDetailsEventArgs__.
          

* __LoadingRowDetails__: Occurs when the row details are being loaded. The type of the passed event arguments is __GridViewRowDetailsEventArgs__.
          

### Column Resizing Events
        

* __ColumnWidthChanging__: Occurs when the column is being resized. Can be canceled. The type of the passed event arguments is __ColumnWidthChangingEventArgs__

* __ColumnWidthChanged__: Occurs after the resize is complete. The type of the passed event arguments is __ColumnWidthChangedEventArgs__

[Read more]({%slug gridview-column-resize-event%})

### Other
      

* __AutoGeneratingColumn__: Occurs each time new column is auto generated by the grid view control. The type of the passed event arguments is __GridViewAutoGeneratingColumnEventArgs__.
        

## GridViewColumn


### Sorting
          

* __SortingStateChanged__: Occurs when the sorting state of the column is changed. The type of the passed event arguments is __RadRoutedPropertyChangedEventArgs<SortingState>__.
            

## GridViewRow


### Data Events
          

* __BindingValidationError__: Occurs when a data validation error is reported by a binding source. The type of the passed event arguments is __ValidationErrorEventArgs__.
            

### Selection Events
          

* __Selected__: Occurs when the grid row is selected. The type of the passed event arguments is __RoutedEventArgs__.
            

* __Unselected__: Occurs when the grid row is deselected. The type of the passed event arguments is __RoutedEventArgs__.
            

### Other
          

* __Loaded / Unloaded__

* __IsExpandedChanged__: Occurs when __GridViewRow__ changes its __IsExpanded__ state. The type of the passed event arguments is __RoutedEventArgs__.
            

## GridViewCell


### Data Events
          

* __BindingValidationError__: Occurs when a data validation error is reported by a binding source. The type of the passed event arguments is __ValidationErrorEventArgs__.
            

### Edit Events
        

* __IsEditorVisibleChanged__: Occurs when the cell editors has visibility changed. The type of the passed event arguments is __RoutedPropertyChangedEventArgs<bool>__.
          

## See Also

 * [Validation]({%slug gridview-events-validation%})