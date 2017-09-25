Go To: `Edit Chart Properties -> Show Advanced Properties`

Edit the following property:

#

* `tooltip.positioner`

```javascript
function(width,height,point) { 
  return {
    x: point.plotX, 
    y: point.plotY 
  } 
}
```
