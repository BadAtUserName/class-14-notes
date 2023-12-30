# class-14-notes
Class 14 notes

Css transforms

Transforms
Transform property comes in two different setting 2d and 3d both have own props and vals. 
II. Transform Syntax
	A. Transform prop simple. 
		1. Includes transform prop followed by the val 
		2. Val specs the transform type followed by a spec amount of inside paren
		div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

	B. Transform prop incl multi vendors refined to gain best support across browsers.

III. 2D Transforms
	A. Elements may be distorted or transformed on both a 2D plane or a 3D plane.
		1. 2d works with x’s and y’s aka horizontal and vertical axes
	B. 2D rotate
		1. The transform property accepts a handful of different vals the rotate val provides ability to rotate from 0-360 degrees.
		2. Default rotation position is 50% 50% both horizontal and vertical
	C. 2D scale
		1. Using scale value with transform prop allows to change the append size of an element.
		2. Default scale val is 1 therefore any val between .99 & .01 makes element appear smaller.
		3. Any val greater than or equal to 1.01 makes eel appear larger
		4. Is possible to scan only height or width using scaleX and scaleY

D. 2d Translate
		1. Translate works like relative positions pushing and pulling an element in different directions without interrupting the normal flow of the document. 
	E. 2D skew
		a. Last transform in val group used to distort element on horizontal axis vert axis or both. 
		b. Syntax is similar to that of the scan and translate vales

IV. Combining transforms
	A. Common for multi transforms to be used at once.
		1. To combine transform probs list the transform vals within the transform prop one after the other without the use of commas.
		2. Do not use multiple transform declaration it will not work each dec will overwrite the one above. 
	B. Behind every transform there is a matrix explicitly defining the behavior of the behavior of the transform. 
V. Transfer origin
	A. As previously mentions the default of transform origin is the dead center of an element. Both 50 hor and 50 vert. 
	B. Transform origin can be used to adjust the mentioned above. 
		1. Prop can accept one or two vals when only one is spec’d will be used for both. 
		2. Does have issues can run into some issues when when using translate transform vale. 
			a. Both attempt to position the element their vals can collide

VI. Perspective
	A. In order for 3D transforms to work the elements need perspective think vanishing point. 
	B. Using the perspective all within the transform property on Indi element while the other includes using the perspective prop on parent element residing over child elements being transformed 

C. Using perspective val within transform prop works great.
		1. If wanting to use on multi elements use it on parent 
	D. Perspective depth val. 
		1 perspective val can be set as none or a length of measure the none val turns off any perspective. 
		2. The length val will set the depth of the persecutive
			a. The higher the val the val the further away the perspective. 	


Transitions and Animations

For transitions to take place an element must have a change in state.
4 states
Hover
Focus
Active
Target
	
B. Four transition related properties in total 
		1. Transition-property
		2. Transition-duration
		3. Transition-timing-fucnction 
		4. Transition-delay 

C. Transitional Properts
		1. Transition-property determines exactly what properties will be altered in conjunction with the other transitions properties. 
		2 by default all props within elements different states will be altered upon change. 
			a. Only properties identified within the transition-property val will be affected by any transitions 
		3. If multiple propertied need to be transitioned they may be separated by comma within the transition-prop value. 
			a. Additionally the keyword value all may be used to transition all properties of an element.

D. Transition duration
		1.transition-duratio Can take seconds or milliseconds. 

E. Transition Timing
		1. Transition-timing-function property is used to set the speed in which a transition will moved. Knowing the duration from the transition-duration property a transition can have multi speeds within a single duration. 
		2. Popular keyword values. 
			a. Linear
			b. Ease-in
			c. Ease-out
			d. Ease-in-out
		3. Linear moves from side to side
		4. Ease-in slowly speeds up though the transition
		5. Ease-out starts quickly an slows down. 
		6. Ease-in0out transition starts slowly speeds up in the middle then slows down again before ending. 
		7. Each timing function has a cubic-bezier curve behind it. Which can be set
			a. cubi-bezier(x1, y1, x2, y2)
			b. Additional vals include
				i. Step-start
				ii. Step-stop
				iii. steps(number_of_steps, direction
		8. Transient Delay
			a. Delay sets. Time value that determines how long a transition should be stalled before executing. 

F. Shorthand transitions
		1. Transition
		2. Transition-property
		3. Transition-duration
		4.transition-timing-function
		5. Transition-delay
		6. Set the all at one using commas


G. Animations
		1. Animations keyframe
			a. To set multiple points at which an element should undergo a transition use @keyframes rule. 
			b. @keyframses includes animation name, any animation breakpoints, and props intended to be animated. 

PLEASE SEE THIS LINK FOR MORE ON ANIMATIONS

Class 14 reading questions

CSS TRANSFORMS

What does a CSS transform allow the developer to do to an element
	a. Css transform allows us to rotate, scale, skew, or translate an element. 
Provide an example of a transform and how you could see that being used on a website.
	a. Using rotate could highlight a graphic/shape of interest to the user and keep your page from looking too static. 

CSS TRANSITIONS & ANIMATIONS

What does a css transition allow the dev to do to an element. 
	a. A transition has the ability to change the appearance and behavior of an elements when a state of change occurs, like it’s hovered, active, targeted, or focused. It must have a change of state to work

2 how does a css animation differ from a css transition
	a. A transition requires something to change an animation does not.

8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS
	
1. What are some benefits to using css transitions on websites. 
	a. Transitions make things more interesting, rather than something being a click it has something fun to to along with it, it’s more interactive and more memeroble for the user. 
2. How this topic fit in with your long-term goals? 
	a. It gives me the tools to make my apps/sites a bit more fun and memorable, I think that it really adds growth to my tools as a developer.  

	 	
