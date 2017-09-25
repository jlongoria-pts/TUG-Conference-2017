Go To: `Edit Chart Properties -> Show Advanced Properties`

Edit the following property:

#

* `chart.load.event`

```javascript
(function(H) {
    if(!window._isAppliedHighchartsTooltipFix) {
        H.wrap(H.Pointer.prototype, 'normalize', function(proceed, e) { 
            var e = proceed.call(this, e), 
            container = this.chart.container.parentNode.parentNode.parentNode.parentNode.parentNode, 
            zoom = parseFloat(container.style.transform.replace('scale(', '').replace(')', '')); 
            
            e.chartX = Math.floor(e.chartX/zoom); 
            e.chartY = Math.floor(e.chartY/zoom); 
            
            return e; 
        });
    }

    window._isAppliedHighchartsTooltipFix = true;
})(Highcharts)
```
