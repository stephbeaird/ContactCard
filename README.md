# ContactCard<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Contact Card</title>
		<link rel="stylesheet" type="text/css" href="styles.css">
		<script type="text/javascript" src="https://code.jquery.com/jquery-3.2.1.js"></script>
		<script type="text/javascript">
			$(document).ready(function(){

				var first = $("#first").val();
				var last = $("#last").val();
				var desc = $("textarea").val();

				$('#contact').append("<div id= 'card'><p>" + first + " " + last +"</p><p id= 'back'> " + desc +"</p></div>");


				$("#first").val("");
				$("#last").val("");
				$("#desc").val("");	

				$(document).on('click', '#card' function(){
					$(this).children().toggle();ß	®
				})
			});
		</script>
	</head>
	<body>
		<div class="wrapper">
			<div id="contact">
				<h3>Jayne Doe</h3>
				<p>Click for description!</p>
				<!--<p>Jayne is a very talented programmer with a specific talent with JQuery!</p>-->			
 				<h3>Paul Smith</h3>
 				<p>Click for description!</p>
				<!--<p>Paul has a bright future with Data Analyzation!</p>-->		
				<h3>Sally Parker</h3>
				<p>Click for description!</p>
				<!--<p>Sally has a great attitude, especially when it comes to Javascript!</p>-->		
			</div>
			<div id="left">
				<form>
					<br><br>
					<label for="first">First name:</label>
					<input type="text" placeholder="First Name" name="FirstName" id="first">
					<br><br>
					<label for="last">Last name:</label>
					<input type="text" placeholder="Last Name" name="LastName" id="last">
					<br><br>
					<textarea for="desc"></textarea>
					<input id="Description">
				</form>
				<button id="btn">Add User</button>
			</div>
	</body>
</html>
body{
	width: 940px;
	font-family: 'arial';
}

form{
	text-align: left;
	margin-left: 30px;
}

button{
	margin-left: 115px;
	margin-top: 12px;
}

.wrapper{
	position: absolute;
	margin-left: 400px;
	width: 300px;
}

#contact h3{
	text-align: center;
	font-family: 'arial';
}

#contact p{
	border: 1px solid black;
	padding: 30px;
	text-align: center;
}

#left{
	margin-left: 100px;
}
