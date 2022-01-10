<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1" />
   <title>Red Ball Survey</title>
   <link href="rb_reset.css" rel="stylesheet" />
   <link href="rb_styles.css" rel="stylesheet" />
   <link href="rb_formst.css" rel="stylesheet" />
   <script src="rb_formsubmit.js"></script>

</head>

<body>
   <header>
      <img src="rb_logo.png" alt="Red Ball Pizza" id="logoimg" />
      <nav> <a id="navicon" href="#"><img src="rb_navicon.png" alt="" /></a>
         <ul>
            <li><a href="#">home</a></li>
            <li><a href="#">menu</a></li>
            <li><a href="#">directions</a></li>
            <li><a href="#">coupons</a></li>
            <li><a href="#">orders</a></li>
            <li><a href="#">catering</a></li>
            <li><a href="#">reviews</a></li>
         </ul>
      </nav>
   </header>
   <section>
      <h1>Customer Survey</h1>
      <p>Thank you for taking our customer survey. Your response 
         helps Red Ball Pizza maintain the tradition that has made 
         us the top-rated pizzeria in the metro area.
         All participants are automatically entered into a monthly
         drawing to receive a <em>Red Ball Express PizzaFest</em> containing 
         two large pizzas, a 2-liter soda, and a side 
         order of chicken wings. Check your e-mail inbox for 
         contest results. </p>
      <p>Surveys are private and confidential. Red Ball 
         Pizza will not share your contact information with third 
         parties, <em>ever</em>. </p>
      <p>Required values are marked by an asterisk (*)</p>
      
      <form id="survey" action="http://www.example.com/redball/survey" method="post">
      	<fieldset id="custInfo">
      		<legend>Customer Information</legend>
      		
      		<div class="formRow">
      			<label for="name">Name*</label> 
      			<input name="custName" id="name" type="text" placeholder="first and last name" required/>
      		</div>
      		
      		<div class="formRow">
      			<label for="street">Street address</label>
      			<input name="custStreet" id="street" type="text" />
      		</div>
      		
      		<div class="formRow">
      			<label for="city">City</label>
      			<input name="custCity" id="city" type="text" value="Ormond Beach" />
      		</div>
      		
      		<div class="formRow">
      			<label for="state">State</label>
      			<input name="custState" id="state" type="text" value="FL"/>
      		</div>
      		
      		<div class="formRow">
      			<label for="zip">Postal Code</label>
      			<input name="custZip" id="zip" type="text" placeholder="nnnnn (-nnnn)"/>
      		</div>
      		
      		<div class="formRow">
      			<label for="phone">Phone number</label>
      			<input name="custPhone" id="phone" type="tel" placeholder="(nnn) nnn-nnnn"/>
      		</div>
      		
      		<div class="formRow">
      			<label for="mail">Email*</label>
      			<input name="custEmail" id="mail" type="email" />
      		</div>
      		
      		<div class="formRow">
      			<label for="info">Where did you hear about us?</label>
      			<select name="infoSrc" id="info" size="5" multiple>
      				<option value="internet">Internet</option>
      				<option value="mag">Magazine</option>
      				<option value="news">News</option>
      				<option value="word">World of Mouth</option>
      				<option value="other">Other</other>
      			</select>
      		</div>
      		
      		<div class="formRow">
      			<label for="dish">What's your favorite dish?</label>
      			<input name="favDish" id="dish" type="text" list="dishType"/>
      			<datalist id="dishType">
      				<option value="Anitpasto Pizza"/>
      				<option value="Big Kahuna Pizza" />
      				<option value="BBQ Chicken Pizza" />
      			</datalist>
      		</div>
      		
      		<div class="formRow">
      			<label for="dineSpine">How many times do you dine out per month?</label>
      			<input name="dineOut" id="dineSpin" type="number" value="1" step="1" max="20" min="1"/>
      		</div>
      		
      		<input name="mailMe" id="mailCB" value="yes" type="checkbox" />
      		<label for="mailCB">Add me to your mailing list for great coupon and specials!</label>
      		
      	</fieldset>
      	
      	
      	<fieldset id="expInfo">
      		<legend>Share Your Experience at Red Ball Pizza</legend>
      		
      		<div class="formRow">
      			<label for="visit">Date of visit</label>
      			<input name="visitDate" id="visit" type="date"/>
      		</div>
      		
      		<div class="formRow">
      			<label for="order">Order type</label>
      			<select name="orderType" id="order">
      				<option value="order1">Carry out</option>
      				<option value="order2">Delivery</option>
      				<option value="order3">Dine in</option>
      				<option value="order4">Take 'n bake</option>
      			</select>
      		</div>
      		
      		<div class="formRow">
      			<label>Was your service friendly</label>
      			<fieldset class="optGroup">
      				<label for="fYes">Yes</label>
      				<input name="sFriend" id="fYes" value="yes" type="radio" />
      				
      				<label for="fNo">No</label>
      				<input name="sFriend" id="fNo" value="no" type="radio" />
      			</fieldset>
      		</div>
      		
      		<div class="formRow">
      			<label>Was your order correct?</label>
      			<fieldset class="optGroup">
      				<label for="cYes">Yes</label>
      				<input name="oCorrect" id="fYes" value="yes" type="radio" />
      				
      				<label for="cNo">No</label>
      				<input name="oCorrect" id="fNo" value="no" type="radio" />
      			</fieldset>
      		</div>
      		
      		<div class="formRow">
      			<label>Was your food hot?</label>
      			<fieldset class="optGroup">
      				<label for="hYes">Yes</label>
      				<input name="foodHot" id="fYes" value="yes" type="radio" />
      				
      				<label for="hNo">No</label>
      				<input name="foodHot" id="fNo" value="no" type="radio" />
      			</fieldset>
      		</div>
      		
      		<div class="formRow">
      			<label for="rangeBox">Rate the overall service<br />(0=poor, 10=great)</label>
      			0<input name="serviceRate" id="rengeBox" type="range" value="5" step="1" min="0" max="10"/>
      			10
      		</div>
      		
      		<label for="commentBox">Tell us more about your experience!</label>
      		<textarea name="custExp" id="commBox"></textarea>
      		
      	</fieldset>
      	
      	<div id="buttons">
      		<input type="submit" value="Submit My Survey" />
      		<input type="reset" value="Cancel" />
      	</div>
      	
      </form>

     
   </section>
   <footer>
      <h1>ORDER</h1>
      <a href="#">Specials</a> <a href="#">Pizza</a> <a href="#">Pasta</a> <a href="#">Wings</a> <a href="#">Sides</a> <a href="#">Salads</a> <a href="#">Drinks</a> <a href="#">Desserts</a>
      <h1>ABOUT US</h1>
      <a href="#">Our Story</a> <a href="#">Blog</a> <a href="#">Catering</a> <a href="#">School Lunches</a>
      <h1>CUSTOMER SERVICE</h1>
      <a href="#">Gluten Free Crusts</a> <a href="#">Contact Us</a> <a href="#">FAQs</a>
      <h1>MY ACCOUNT</h1>
      <a href="#">Create an Account</a> <a href="#">Sign In</a> <a href="#">Order Status</a>
      <h1>NUTRITION</h1>
      <a href="#">Nutrition Information</a> <a href="#">Food Allergen</a> <a href="#">Gluten Free Pizza</a>
      <h1>POLICIES</h1>
      <a href="#">Privacy Policy</a> <a href="#">Terms of Use</a>
      <address>
      Red Ball Pizza <br />
      811 Beach Drive <br />
      Ormond Beach, FL  32175 <br />
      (386) 555 - 7499
      </address>
   </footer>
</body>
</html>
