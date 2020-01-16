---
EventForAction: ..\4 Events\exporting.md
default: null
type: function(e)
---
---
##### shortDescription
A handler for the [exporting](/api-reference/20%20Data%20Visualization%20Widgets/BaseSparkline/4%20Events/exporting.md '{basewidgetpath}/Events#exporting') event.

##### param(e): object
Information about the event.

##### field(e.component): object
The widget <a href="{basewidgetpath}/Methods/#instance"></a> instance.

##### field(e.element): jQuery
The widget's container.

##### field(e.model): object
Data that is available for binding against the element. Available only in Knockout and AngularJS approaches.

##### field(e.fileName): string
The name of the file to which the widget is about to be exported.

##### field(e.cancel): boolean
Assign <i>true</i> to this field if you need to prevent exporting.

---
To perform a custom action before data from the widget is exported, assign a function to this option. Within this function, you can use the object passed to it as the parameter. For example, using the **cancel** field of this object, you can cancel exporting.

#####See Also#####
- [onExported](/api-reference/20%20Data%20Visualization%20Widgets/BaseSparkline/1%20Configuration/onExported.md '{basewidgetpath}/Configuration#onExported') - allows you to notify an end user when exporting is completed.
- [onFileSaving](/api-reference/20%20Data%20Visualization%20Widgets/BaseSparkline/1%20Configuration/onFileSaving.md '{basewidgetpath}/Configuration#onFileSaving') - allows you to access exported data and/or prevent it from being saved into a file on the user's local storage.