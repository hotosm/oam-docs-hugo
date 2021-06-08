---
title: Constructs
type: pages
bookShowToC: true
---

## Flag

### Regular

![](/content/design/regular-flag.png)

```html
<article class="flag-construct flag-construct--align-top">
  <div class="flag-construct__media">
    <img alt="flag-construct image" width="320" height="320" src="{{ site.baseurl }}/assets/graphics/content/design/earth-img-square.jpg" />
  </div>
  <div class="flag-construct__body">
    <h3>This is a title</h3>
    <p>Morbi eget mattis ipsum. Donec massa nibh, bibendum at sem eu purus. Nunc in tortor eu tellus ultricies euismod.</p>
    <p>Duis massa mi, pharetra eu nisl non, scelerisque laoreet diam. Fusce in malesuada justo. Aenean vulputate mi a pharetra lorem ipsum tristique.</p>
    <button class="button button--achromic" type="button"><span>Action</span></button>
  </div>
</article>
```

### Reverted

![](/content/design/reverted-flag.png)

```html
<article class="flag-construct flag-construct--align-top">
  <div class="flag-construct__body">
    <h3>This is a title</h3>
    <p>Morbi eget mattis ipsum. Donec massa nibh, bibendum at sem eu purus. Nunc in tortor eu tellus ultricies euismod.</p>
    <p>Duis massa mi, pharetra eu nisl non, scelerisque laoreet diam. Fusce in malesuada justo. Aenean vulputate mi a pharetra lorem ipsum tristique.</p>
    <button class="button button--achromic" type="button"><span>Action</span></button>
  </div>
  <div class="flag-construct__media">
    <img alt="flag-construct image" width="320" height="320" src="{{ site.baseurl }}/assets/graphics/content/design/earth-img-square.jpg" />
  </div>
</article>

```


### Full bleed

![](/content/design/full-bleed-flag.png)

```html
<figure class="bleed-full">
  <img class="image-full" width="2560" height="768" alt="Full bleed image" src="{{ site.baseurl }}/assets/graphics/content/design/earth-img-wide.jpg" />
</figure>
```

