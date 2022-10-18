the layout is compoesed of various properties such as title, font, etc.. those properties may change depending on the type of the trace.

```javascript
var layout = { 
	title: 'Responsive to window\'s size!', 
	font: {size: 18} 
};
```
this can also be used with legend and font which are other objects within it 
```javascript
var layout = {
  xaxis: {
	title: 'GDP per Capita', 
	showgrid: false, 
	autorange: true,
	gridwidth: 1,
	zeroline: false,
	tickangle: 60,
    range: [ 0.75, 5.25 ]
  },
  yaxis: {
	title: 'Percent', 
	showline: false,
	zerolinecolor: 'rgb(255, 255, 255)', 
	zerolinewidth: 2,
    range: [0, 8]
  },
  legend: {
	width: 500, 
	height: 500,
    y: 0.5,
    yref: 'paper',
    font: {
      family: 'Arial, sans-serif',
      size: 20,
      color: 'grey',
    }
  },
  paper_bgcolor: 'rgba(245,246,249,1)', 
  plot_bgcolor: 'rgba(245,246,249,1)', 
  width: 600, 
  height: 600,
  showlegend : false,
  title:'Data Labels on the Plot'
};

```
#### Bar charts
If you are using a reace with a type of bar you can either choose a barmode object of:
- stack
- group
and you can use the property of :
- bargap
- bargroupgap (if you have barmode of group)

for plots of type "box" the following object can be used to make them horizontal and group the output 
```javascript
var layout = { 
	yaxis: { title: 'normalized moisture', zeroline: false },
		boxmode: 'group' 
	};
```

#### Histograms
for a histogram in order to put the two traces on top of each other
```javascript
var layout = {barmode: "overlay"};
```
to stack them up
```javascript
var laout = {barmode : "stack"};
```
then to group the plots you can use
- bargap: 0.05, 
- bargroupgap: 0.2,