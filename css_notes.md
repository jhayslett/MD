#CSS Notes
###Written by jhayslett  
###Last Updated: 09/18/2016
___  
##Positions
**static**  
  - defualt positioning for html elements  
  - considered to be not positioned  

**relative**  
  - behaves same as static, but is positioned  
  - can be altered by top, right, left, and bottom  

**fixed**  
  - positioned to the viewport window  
  - stays in the same place if scrolled  
  - does not let area where it would have been in normal document flow  

**absolute** - parent element must be positioned to be based off of
  - acts similar to fixed, but it's positioned to the next parent element that is positioned
  - a positioned element is anything that isn't static
___

##FAQS

**How can I center an element vertically and horizontally?**

**Vertical Middle** 

1 - Absolute position  
```css```
.container { // The parent element that it will be based off of needs to be positioned  
    position: absolute;  
    top: 50%;  
    left: 50%;                                     // this is to make up for half the  
    transform: translateX(-50%) translateY(-50%);  // height and width of the element 
}                                                  // from the 50% top and left  
```  

This method seems simple and straightforward.

2 - Flexbox  

```css```
html, body, .container {  
    height: 100%;  
}  
.container {  
    display: flex;  
    align-items: center;  
    justify-content: center;  
}  
```
**Horizontal Center**  
```css```  
.center {  // The parent element must have a width set for this to take affect
  margin: auto;
}  
```  
