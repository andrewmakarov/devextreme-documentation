---
default: undefined
type: function(aggregationInfo, series)
---
---
##### shortDescription
Specifies a custom aggregate function. Applies only if the [aggregation method](/api-reference/20%20Data%20Visualization%20Widgets/dxChart/5%20Series%20Types/CommonSeries/aggregation/method.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxChart/Configuration/series/aggregation/#method') is *"custom"*.

##### param(aggregationInfo): chartPointAggregationInfoObject
An object with information about the aggregation interval and the data objects that fall within it.

##### param(series): chartSeriesObject
The series to which the aggregate function is being applied.

##### return: Object|Array<Object>
One or several aggregated data objects. Should have the same structure as the original data objects.

---
---
##### jQuery

    <!--JavaScript-->
    $(function() {
        $("#chartContainer").dxChart({
            // ...
            series: [{
                // ...
                aggregation: {
                    enabled: true,
                    method: "custom",
                    calculate: function (aggregationInfo, series) {
                        var dataObjects = aggregationInfo.data;
                        var result = { }; // or [ ]
                        // ...
                        // Aggregate the data objects here
                        // ...
                        return result;
                    }
                }
            }]
        });
    });

##### Angular

    <!--HTML-->
    <dx-chart ... >
        <dxi-series ... >
            <dxo-aggregation
                [enabled]="true"
                method="custom"
                [calculate]="customAggregateFunc">
            </dxo-aggregation>
        </dxi-series>
    </dx-chart>

    <!--TypeScript-->
    import { DxChartModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        customAggregateFunc (aggregationInfo, series) {
            let dataObjects = aggregationInfo.data;
            let result = { }; // or [ ]
            // ...
            // Aggregate the data objects here
            // ...
            return result;
        };
    }
    @NgModule({
        imports: [
            // ...
            DxChartModule
        ],
        // ...
    })

---