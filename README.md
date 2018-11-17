# Material-design-color-palette
Scss (sass) and css material design color palette to use in your next project. 

![Image](https://i.imgur.com/J5ZQIsd.png)

## Customization
Use sass file to create your custom class names 
sass file orgnized into three parts/steps

 1. Defining all colors and turn the colors to variables
``` 
$Red-500 : #F44336; 
```
 2. Turn color variables to a color map
``` 
$color-map: (
	Red-50 : $Red-50 
)
```
 3. Using map turn all colors to background-color, Color and
 border-color with the same name
``` 
@each $color-key, $color-var in $color-map {
	.md-bg--#{$color-key} {
		background-color: $color-var;
	}
}
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA5NTU4NjUyOCwxMTIzOTI5MzI5LDE2OD
QzMjY4ODcsMjExMzcyODIyOSw0NDA0MzIzNDgsODYxMjU2ODk5
LC0xMzE5NzExMTM1LC0xODA2MTIyNDAxXX0=
-->