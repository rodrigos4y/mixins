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
For example

```
@include theme-color(7, 180);
```

Results in this CSS
```
.bg-2 {
  background: #003333;
}

.bg-3 {
  background: #004d4d;
}

.bg-4 {
  background: #006666;
}

.bg-5 {
  background: teal;
}

.bg-6 {
  background: #009999;
}

.bg-7 {
  background: #00b3b3;
}

```

Look the result here: [Theme Color](https://rdfreitas.com.br/mixins/theme-color).

## Versioning

### Version 1.0.0
- Create the mixin for Theme Color

## Contributing
Find on our [issues](https://github.com/rodrigos4y/mixins/issues) the next steps of the project ;)
Want to contribute? Follow these recommendations.


