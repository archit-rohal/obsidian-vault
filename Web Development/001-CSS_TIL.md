## TIL 
tag: #tilhtml
- Inline styles, usually, should almost never be used, reason being separation of concerns and semantics most of the time and - 
	- ==separation of concerns== in html and css
- What's the meaning of ==rel="stylesheet"== in the syntax (`<link href="style.css" rel="stylesheet />`) when linking CSS stylesheets to HTML. Ans - it is to tell, ahead of time, HTML that this is a CSS stylesheet 
- Using class and ID selectors is better than using a nested descendant selector in place of it because using nested descendant selectors is akin to encoding the HTML structure into the CSS selectors, and that can make our code hard to maintain in the future. Ex -
	 ```css
      	article header p {
		font-style: italic; 
		}	
	 ```
	 the use of two descendant elements - header and p is inefficient here because we're borrowing the structure of the HTML file here
- Conventionally two-worded names for class and ID attributes inside of HTML elements are used with a 'dash' ('related-author') in between like this #classid- 
	 ```html
			<p class="related-author">Oscar Wilde</p>
	 ```
- Big difference between class and ID (attributes) is that we are not allowed to repeat an ID name once it has been used in the HTML. We can use each ID name only once. Ex - we can't use the id of copyright `id='copyright'` anywhere else in our HTML once it has already been used  #id
- Because id attributes can be used only once, it's a serious limitation considering the future maintainability/expansion of the code and so we hardly use id's in the real world #id 
- Colors in CSS - Between rgb and hexadecimal notation for colors, in practice, we mostly use hexadecimal colors and rgba when we need transparency
- In rgb when colors in all 3 channels are same, we get a grey color
- The `border` property is a special property in that it accepts multiple values like so -  `aside { border: 5px solid #1098ad;}`. It's also called 'shorthand property' because we can use just one property for defining 3 different properties.