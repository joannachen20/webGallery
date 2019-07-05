<html>
<head>
	<title>T H R O U G H M Y E Y E S</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<center>
	<div id="gallery">
		<img src="topview.jpg">
		<img id="empireState" src="empire.jpg">
		<img src="happybones.jpg">
		<img id="water" src="water.jpg">
		<img src="happiness.jpg">
		<img src="dumbo.jpg">
		<img src="met.jpg">
		<img id="coffee" src="coffee.jpg">
		<img src="miss.jpg">
		<img src="bridge.jpg">
	</div>
	</center>

<script>
	alert("Yesterday is history, tomorrow is a mystery, today is a gift of God, which is why we call it the present.")
	var empireState = document.querySelector('#empireState');
	var coffee = document.querySelector('#coffee');
	var water = document.querySelector('#water');
	function dayToNight(event) {
    var currentSource = empireState.getAttribute('src');
    if (currentSource == "empire.jpg") {
        empireState.setAttribute("src", "empire2.jpg");
    } else {
        empireState.setAttribute("src", "empire.jpg");
    }
}
	function sideToTop(event) {
    var currentSource = coffee.getAttribute('src');
    if (currentSource == "coffee.jpg") {
        coffee.setAttribute("src", "coffee2.jpg");
    } else {
        coffee.setAttribute("src", "coffee.jpg");
    }
}
	function viewsToMe(event) {
    var currentSource = water.getAttribute('src');
    if (currentSource == "water.jpg") {
        water.setAttribute("src", "self.jpg");
    } else {
        water.setAttribute("src", "water.jpg");
    }
}
empireState.addEventListener('mouseover', dayToNight);
empireState.addEventListener('mouseout', dayToNight);
coffee.addEventListener('mouseover', sideToTop);
coffee.addEventListener('mouseout', sideToTop);
water.addEventListener('mouseover', viewsToMe);
water.addEventListener('mouseout', viewsToMe);
</script>
</body>
</html>
