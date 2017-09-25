Go To: `Edit Chart Properties -> Show Advanced Properties`

Edit the follwing properties:

#

* `tooltip.headerFormat`:

```javascript
<small>{point.key}</small><table>
```

#

* `tooltip.pointFormat`:

```javascript
<tr>
  <td><svg width='7px' height='5px'><circle fill='{series.color}' r='3.5' cy='2.5' cx='2'></svg></td>
  <td>{series.name}: </td>
  <td></td>
  <td style='text-align:right;'><b>{point.y:.2f}%</b></td>
</tr>
```

#

* `tooltip.footerFormat`

```javascript
</table>
```
