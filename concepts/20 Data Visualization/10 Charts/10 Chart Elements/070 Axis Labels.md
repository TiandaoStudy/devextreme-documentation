Axis labels represent textual values for [axis ticks](/concepts/20%20Data%20Visualization/10%20Charts/10%20Chart%20Elements/080%20Axis%20Ticks/01%20Axis%20Ticks.md '/Documentation/Guide/Data_Visualization/Charts/Chart_Elements/#Axis_Ticks').

![Axis Labels](/images/ChartJS/AxisLabels.png)

Axis labels are generated automatically. However, you can change their settings if your task requires that. Label settings are set using the [label](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/commonAxisSettings/label '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonAxisSettings/label/') object of the **argumentAxis**, **valueAxis** or **commonAxisSettings** configuration object.

	<!--JavaScript-->var chartOptions = {
		commonAxisSettings: {
			label: {
				//...
			}
		},
		//...
	};

The following list provides an overview of label options.

* **Visibility**		
To mark point labels as visible/invisible, use the **label** object's [visible](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/commonAxisSettings/label/visible.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonAxisSettings/label/#visible') property.

* **Intelligent Arrangement**		
If labels overlap each other in certain scenarios (e.g., device rotations, browser resizing or long text after formatting), specify how to resolve this issue using the [overlappingBehavior](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/commonAxisSettings/label/overlappingBehavior '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonAxisSettings/label/overlappingBehavior/') property.

* **Font Settings**		
To specify the required font settings for label text, specify properties of the **label** | [font](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/commonAxisSettings/label/font '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonAxisSettings/label/font/') object.

* **Text Customization and Formatting**			
You can change the way the default text is displayed by labels. For this purpose, use the [format](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/argumentAxis/label/format.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/argumentAxis/label/#format') label property. If it is required, you can set a custom text to be shown by labels. For this purpose, implement a function that returns the required text and assign it to the [customizeText](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/argumentAxis/label/customizeText.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/argumentAxis/label/#customizeText') property of the **label** object. For details on data formatting, refer to the [Data Formatting](/concepts/20%20Data%20Visualization/40%20Common/30%20Data%20Formatting '/Documentation/Guide/Data_Visualization/Common/Data_Formatting/') topic.

* **Label Position**		
You can shift labels closer to or farther from the axis. For this purpose, use the **label** object's [indentFromAxis](/api-reference/20%20Data%20Visualization%20Widgets/10%20dxChart/1%20Configuration/commonAxisSettings/label/indentFromAxis.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/commonAxisSettings/label/#indentFromAxis') property.