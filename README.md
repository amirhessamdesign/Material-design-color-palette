# Material-design-color-palette
Scss (sass) and css material design color palette to use in your next project. 
## Customaztion 
Use sass file to create your custome class names 
sass file orgnized in three parts/steps

 1. Defining all colors and turn the colors to varibales
``` 
$Red-500  :  #F44336; 
```
 2. Turn color varibles to a color map
``` 
$color-map: (
	Red-50  :  $Red-50 
)
```
 3. Using map turn all colors to background-color, Color and
    border-color with same name
``` 
@each  $color-key, $color-var  in  $color-map {
	.md-bg--#{$color-key} {
background-color:  $color-var; 

}

}
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk2OTY3NDE4MSwtMTgwNjEyMjQwMV19
-->