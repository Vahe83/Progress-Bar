# Progress Bar And Widt / Height In JavaScript By Amur
## Example
<img src="img/progress.gif" style="width: 100%; max-width: 600px;" />
## Get started

### html
	<div class="circle-1" data-count="85" style="width: 200px;"></div>
	<div class="circle-2" data-count="4,55" style="width: 200px;"></div>
	<div class="circle-3" data-count="70000" style="width: 200px;"></div>
	
	<script type="text/javascript" src="progress.js"></script>
	<!-- or -->
	<script type="text/javascript" src="progress.min.js"></script>

### JavaScript
	let Circle1 = document.getElementsByClassName('circle-1');
	let Circle2 = document.getElementsByClassName('circle-2');
	let Circle3 = document.getElementsByClassName('circle-3');

	let options = {
	    fontColor: '#FFFFFF',
	    fontSize: 18,
	    fontWeight: 900,
	    fillParent: '#6949D7',
	    fillChild: 'transparent',
	    interval: 1000,
	    animated: true,
	    strokeWidthParent: 5,
	    strokeWidthChild: 5,
	    progressColor: '#FE3F44',
	    progressParentCircleColor: '#FFD200'
	};

	new Progress(Circle1, options).inPercent();
	new Progress(Circle2, options).inCount(5);
	new Progress(Circle3, options).inCounter();
	
### JavaScript default options
	{
            fontColor: '#000000',
            fontSize: 16,
            fontWeight: 400,
            fillParent: 'none',
            fillChild: 'none',
            interval: 1000,
            animated: false,
            strokeWidthParent: 3,
            strokeWidthChild: 5,
            progressColor: '#00AAFF',
            progressParentCircleColor: '#E0E0E0',
	}

## Other Opportunities:
### html
	<div class="other" style="width: 200px;"></div>
### javascript
	let parameters = new GeterSeterParameters(elem);
	parameters.Width; // return width
	parameters.Width = 300;
	// or
	parameters.Width = "300px";
	parameters.Height; // return height
	parameters.Height = 200;
	// or
	parameters.Height = "200px";
