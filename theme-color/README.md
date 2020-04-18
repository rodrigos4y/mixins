# Mixin Theme Colors

This mixin is for you who wants create a theme color palette. You can choose a range, color and saturation (he defaults is 100%)

```
@mixin theme-color($number, $hue, $saturation : 100%){
    @for $i from 2 through $number {
        .bg-#{$i} {
            background: hsl($hue, $saturation, $i * 5);
        }
        
    }
}

```
For exxample

```
@include theme-color(7, 180);
```
Look the result here: [Theme Color](https://rdfreitas.com.br/mixins/theme-color).

## Versioning


## Contributing
Find on our [issues](https://github.com/rodrigos4y/mixins/issues) the next steps of the project ;)
Want to contribute? Follow these recommendations.


