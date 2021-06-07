---

title: Iconography
---

The OAM Design System includes a small library of UI icons based off [Collecticons](http://collecticons.io/) to be used on web applications. This icon font can be easily customized using just CSS: size, color, drop shadow, etc.

## Usage

You can place OAM icons just about anywhere using the respective CSS class. The icon library is designed to be used with inline elements (we like the `<i>` tag for brevity, but using a `<span>` is more semantically correct). 
```html
<button><i class="oam-ds-icon-circle-information"></i> Info</button>
```

You can also use `scss` extends for a semantic approach:
```html
<button class="bttn-info">Info</button>
```
```scss
.bttn-info {
  :before {
    @extend %oam-ds-icon-circle-information;
  }
}
```

The advantage of the semantic approach is that there's no need for any extra markup and it is possible to choose on which pseudo-element to apply the icon.
