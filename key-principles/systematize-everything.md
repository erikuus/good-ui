# Systematize everything 

Instead of hand-picking values from a limitless pool any time you need to make a decision, start with a smaller set of options. 

## Colors

**Primary colors**

Most sites need one, maybe two colors that are used for primary actions, active navigation elements, etc.



**Accent colors** 

On top of primary colors, every site needs a few accent colors for communicating different things to the user. 



**Greys** 

Text, backgrounds, panels, form controls. 



## Shadows

**Small**

You might use a smaller shadow for something like a button. 

 

**Medium**

Medium shadows are useful for things like dropdowns. 




**Large**

Large shadows are great for modal dialogs. 



## Sizes

You shouldn’t be nitpicking between 1px difference when trying to decide on the perfect size for an element or a space between elements.



## Presets

Systematize everything: Font size, Font weight, Line height, Color, Margin, Padding, Width, Height, Box shadows, Border radius, Border width, Opacity. If your framework supports presets, package up your set of options for easy use.

```
// tailwind.config.js
module.exports = {
  presets: [
    require('./custom.preset.js')
  ],
  ...
}

// custom.preset.js
module.exports = {
	theme: {
		screens: {
			'tablet': '960px',
			'desktop': '1248px',
		},
		colors: {
			white: '#FFFFFF',
			purple: '#3F3CBB',
			midnight: '#121063',
			metal: '#565584',
			'tahiti-blue': '#3AB7BF',
			'cool-white': '#ECEBFF',
			'bubble-gum': '#FF77E9',
			'copper-rust': '#78DCCA'
		},
		boxShadows: {
			sm: '0px 2px 4px 0px rgba(11, 10, 55, 0.15)',
			lg: '0px 8px 20px Opx rgba(18, 16, 99, 0.06)'
		},
		fontSize: {
			xs: ['14px', {
				lineHeight: '24px', 
				letterSpacing: '-0.03em'
			}],
			sm: ['16px', {
				lineHeight: '28px', 
				letterSpacing: '-0.03em'
				}],
			lg: ['18px', {
				lineHeight: '28px',
				letterSpacing: '-0.03em'
			}],
			xl: ['24px', {
				lineHeight: '36px',
				letterSpacing: '-0.03em'
			}],
			'2xl': ['36px', {
				lineHeight: '48px',
				letterSpacing: '-0.032em'
			}],
			'3xl': ['48px', {
				lineHeight: '56px', 
				letterSpacing: '-0.032em' 
			}],
			'4xl': ['56px', {
				lineHeight: '64px',
				letterSpacing: '-0.032em'
			}],
			'5xl': ['80px', {
				lineHeight: '80px',
				letterSpacing: '-0.032em'
			}]
		},
		fontFamily: {
			satoshi: 'Satoshi, sans-serif',
			inter: 'Inter, sans-serif'
		}
	}
}
```
