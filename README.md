#HTML5 Baseplate

##ABOUT:

**HTML5 Baseplate** is a collection of the best, most useful bootstraps, resets, boilerplates and snippets out there.

Add in a bit of SMACSS and OOCSS influence and some of the best practices that I have adopted over the past few years and you get the perfect starting point for any project.

I will be adding to this README in the future, covering each piece and portion in detail, but for now, poke around and enjoy, use, manipulate, do whatever you'd like to make this your own. I welcome comments and feedback.

##UPDATE:  

I decided to add some basic responsive aspects to the Baseplate. I included a cookie-cutter navigation example and set the `<aside>` to the right. I'm really trying to keep the code to a minimum and not make assumptions about how this should be used, but I wanted the demo to have at least a <em>little</em> life to it.  

###DEMO 

http://maxquattromani.com/HTML5-baseplate/

Here is a list of sources I leaned on while building baseplate:


##SOURCES:

ARIA				:: http://www.w3.org/WAI/intro/aria
CSS Tricks			:: http://css-tricks.com  
CSSWizardry			:: http://csswizardry.com/  
Entypo Pictograms	:: http://entypo.com  
HTML5 Boilerplate	:: http://html5boilerplate.com  
HTML5 Reset			:: http://html5reset.org  
Max Voltar			:: http://maxvoltar.com/archive/-webkit-font-smoothing/  
Modernizr			:: http://modernizr.com/  
Normalize			:: http://necolas.github.com/normalize.css  
Nicole Sullivan		:: https://github.com/stubbornella/oocss/wiki  
Remy Sharp			:: http://remysharp.com/2009/01/07/html5-enabling-script/  
SMACSS				:: http://smacss.com/  
Tim Kadlec			:: http://timkadlec.com/2012/10/ie10-snap-mode-and-responsive-design/  
Twitter Bootstrap	:: http://twitter.github.com/bootstrap/  

##CSS Best Practices Employed

###Formatting 

Space between selector and opening curly brace.  
Space after opening curly brace and declaration (single line) or line-break after opening curly brace (multi-line).    
Multiple selectors are separated by a comma and line-break.  
One selector/one attribute/one line - everything else is multiline (one exception: I break this rule for the reset just to keep it under control).  
  
	EX:	.someDiv { color: #222; }  
	   
		.someOtherDiv,
		.someAdditional Div {
			color: #222;  
			margin: 0 auto;  
		}  
		
###Declaration Organization  

I use the following ordering method for my declarations:  

Box (Display, Float, Position, Left, Top, Width, Margin, Padding, etc.)  
Border  
Background  
Text  
Other  

###Commenting  

Section comments are styled thusly:  

/* 	==========================================================================  
	Section  
   	========================================================================== */   
     
Section chunks get styled as such:  

/* 	==========================  
   	Chunk  
   	========================== */  
   
and Hints get styled like this:  

/* Hint */  

##HTML Best Practices Employed  

###Attribute Order  

* Class
* ID
* Data-*
* for | |type | href  

	EX: <a class="" id="" data-name="" href="">[link]</a>

##Code Choices Explained  

###Media Queries  

I made the decision to limit the media queries in Baseplate to three (3) resolutions only. The reasoning for this is simple; I had found myself constantly chasing fixes for devices (640px here, 1280px there, back to 800px for something else), it's just too much to try to control. By deciding at the planning stage that your design/site will break layout at distinct points allows the opportunity to anticipate problems from the get-go.  

Most smartphones sit at or under 480px, tablets (in portrait mode) are mostly 768px, and standard desktops/laptops (and tablet landscape modes) hang out in the 1024px range or above. 

###UPDATE:  

**I have changed my media queries from pixel measurements to em's. After some research I think that this offers more flexibility for smaller screens; especially in regards to tablet/smartphone zooming.**   

Of course you're welcome to make whatever changes you like. This makes sense to me and allows me to define how the site will work better upfront to the designers, PM's, and business owners before I lay down the first line of code.   

###ARIA  

I am using ARIA role attributes as best as possible. By setting these upfront, HTML5 Baseplate "make(s) it possible to provide an enhanced user experience for people with disabilities when using internet applications with assistive technologies."  

##Find and Highlight Mistakes in HTML  

Included in main.css is Eric Meyer's Diagnostic CSS code. This little tidbit will let you know if you've left any empty classes hanging around or if you've used a deprecated selector. Very handy piece of code, although you may want to remove it from your final production stylesheet just for the sake of minifying your code as much as possible.

