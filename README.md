# food-order
app
<!DOCTYPE html>
<html>
<head>
<title> Foods</title>
<link rel="stylesheet" type="text/css" href="food.css">
</head>
<body>
	<h1>Food World</h1>
	<nav>
		<ul>
			<a href="#"><li>Home</li></a>
			<a href="#"><li>Order</li></a>
			<a href="#"><li>Near</li></a>
			<a href="#"><li>About</li></a>
		</ul>
	</nav>

	<section class="items">
		<div class="item">
			<img src="food 1.jpg">
			<h4>Chicken curry</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 2.jpg">
			
			<h4>Chicken wings</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 3.jpg">
			
			<h4>Korean Fried Chicken</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 4.jpg">
			
			<h4>Chicken dinner</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 5.jpg">
			
			<h4>Grilled</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 6.jpg">
			<width = 20px>
				<length= 50px>
			<h4>Whole Roasted Chicken Dinner</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 7.jpg">
			
			<h4>Pizza</h4>
			<button>Order</button>
		</div>
		<div class="item">
			<img src="food 8.jpg">
			
			<h4>Buger</h4>
			<button>Order</button>
		</div>
			</div>
		<div class="item">
			<img src="food 9.jpg">
			
			<h4>Tea</h4>
			<button>Order</button>
		</div>
	</section>
</body>
	</html>
	*{
	margin: 0;
	padding: 0;
	font-family: sans-serif;
	box-sizing: border-box;
}
h1{
	text-align:  center;
	color:  blue;
	padding: 20px;
}
nav{
	background-color: white;
	display:  grid;
	place-items: center;
}
nav ul{
	list-style-type: none;
}
nav ul a{
	display: inline-block;
	padding: 20px;
	text-decoration: none;
	color: #000;
	transition: 0.2s ease-in;
	font-size: 18px;
}
nav ul a:hover{
	background-color: green;
	color:  white;
}
.items{
	display: grid;
	grid-template-columns: repeat(3, 1fr);
	padding: 30px 20px;
	grig-colum-gap: 20px;
	grid-row-gap: 30px;
}
.item img{
	width: 100%;
	height: 300px;
	object-fit: cover;
	cursor: pointer;
	transition: 0.2s ease;
}
.item img:hover{
	transform: scale(1.04);
}
.item h4{
	padding: 5px;
	text-align: center;

}
.item button{
	padding: 5px 30px;
	border: none;
	outline: none;
	background-color: green;
	color: white;
	cursor: pointer;
	border-radius:4px ;
	font-size: 20px;
	display: block;
	margin: 0 auto;
	transition:0.2s all ;

}
.item button:hover{
	transform: scale(1.08);
}
@medium screen and(max-width: 1000px){
	item{
		grid-template-columns: repeat(2, 1fr);
	}
}
@medium screen and(max-width: 768px){
	item{
		grid-template-columns: repeat(1, 1fr);
	}
}
