# D3-Transition

<script type="text/javascript">

// Width and height of the SVG object
	let w = 400;
	let h = 175;
	
//Make an SVG Container
var svgContainer = d3.select("div#main")
		.append("svg")
		.attr("width", 400)
		.attr("height", 200)
		.style("border-color", "black")
		.style("border-style", "solid")
		.style("border-width", "0.25px");
		
// Draw the Rectangle
var rectangle = svgContainer.append("rect")
		.attr("x", 50)
		.attr("y", 50)
		.attr("width", 50)
		.attr("height", 50);
		
// Set up the reset button to move it back to 50,50
d3.select("#reset").on("click", function() {
rectangle
		.transition()
		.attr("x", 50)
		.attr("y", 50);
});

d3.select("#start").on("click", function() {
	rectangle
	.transition(); // 
		});
