> NB: Данный скрипт был найден на просторах интернета и использован в своем проекте, в котором мне захотелось добавить поддержку иконок внутри выпадающего списка. Что и было сделано. Создан данный форк.

# EasyDropDown
### A Drop-down Builder For Styled Inputs and Menus (witch supports icons inside option)

### What Is It?

EasyDropDown is a jQuery plugin that effortlessly turns humble <select> elements into styleable drop-down menus for use in forms or general UI/navigation.
	
It's like Chosen but with only the essential features:

+ Clean, semantic markup
+ Form & validation compatibilty
+ Full keyboard control with textual search
+ Inner-scroll for long lists
+ Degradation to native UI on touch devices
+ Fully functional IE8+

###How To Use It

To use, simply include the jquery.easydropdown.min.js script in your page and give your <select> tags the class dropdown:

	<select class="dropdown">
		<option value="1">Option 1</option>
		<option value="2">Option 2</option>
		<option value="3">Option 3</option>
		<option value="4">Option 4</option>
	</select>
	
If you are using labels within the <select> element, identify them with the class label:

	<select class="dropdown">
		<option value="" class="label">Month</option>
		<option value="1">January</option>
		<option value="2">February</option>
		<option value="3">March</option>	
	</select>
	
To build your dropdown with an arbitrary option pre-selected, simply give it the selected attribute as you normally would:

	<select class="dropdown">
		<option value="" class="label">Month</option>
		<option value="1">January</option>
		<option value="2" selected>February</option>
		<option value="3">March</option>		
	</select>
	
Similarly, a dropdown may be disabled with the disabled attribute:

	<select class="dropdown" disabled>
		<option value="" class="label">Month</option>
		<option value="1">January</option>
		<option value="2">February</option>
		<option value="3">March</option>		
	</select>
	
Use witch icons inside option:

	<select class="dropdown">
		<option value="" class="label">Month</option>
		<option value="1" data-icon="/images/icon1.png">January</option>
		<option value="2" data-icon="/images/icon2.png">February</option>
		<option value="3" data-icon="/images/icon3.png">March</option>		
	</select>
	
No custom JS required!

###How To Style It

Either create your own styles to match your design and branding, or use one of our ready made themes. We recommend starting with the default theme and customizing it.

Each drop-down has the following basic markup structure that you can target with your CSS:

	<div class="dropdown">
		<span class="old">
			<select>...</select>
		</span>
		<span class="selected">Option 1</span>
		<span class="carat"></span>
		<div>
			<ul>
				<li>Option 1</li>
				<li>Option 2</li>
				<li>Option 3</li>
				<li>Option 4</li>
			</ul>
		</div>
	</div>
	
