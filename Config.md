to change the scroll behaviour of the plot you can use a scrollzoom of true
```javascript
PLotly.newPLot(data, layout, {scrollZoom : true})
```
you can also set the editable mode to true to edit features of the plot
```javascript
PLotly.newPLot(data, layout, {editable : true})
```
you can also custom the to image button options to allow your image to be donwloaded as an svg
```javascript
var config = {
  toImageButtonOptions: {
    format: 'svg', // one of png, svg, jpeg, webp
    filename: 'custom_image',
    height: 500,
    width: 700,
    scale: 1 // Multiply title/legend/axis/canvas sizes by this factor
  }
};
```
alternatively you can also toggle the display of the modebar to remove it from the plot
```javascript
Plotly.newPlot(data,layout, { displyModebar : true})
```
Additionally, using the following object you can display the edit chart button 
```javascript
var config = { 
	showLink: true, 
	plotlyServerURL: "https://chart-studio.plotly.com",
	linkText: 'This text is custom!'
};
```
with the linktext to customise the text that is displayed at the button right
Also, you can also remove the logo from all the plots, using the following
```javascript
Plotly.newPlot(data,layout, {displaylogo : false})
```
finally you can also controll the responsiveness by using the responsive class as true or false ``{ responsive : true}`` .