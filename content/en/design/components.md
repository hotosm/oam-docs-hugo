---

title: Components
bookShowToC: true
type: pages
---

## Buttons

### Colors

![](/content/design/colors.png)

```html
<button class="button button--achromic" type="button"><span>Achromic</span></button>
<button class="button button--base" type="submit"><span>Base</span></button>
<a class="button button--primary" role="button"><span>Primary</span></a>
<button class="button button--secondary" type="button"><span>Secondary</span></button>
<button class="button button--base-unbounded" type="button"><span>Base unbounded</span></button>
<button class="button button--primary-unbounded" type="button"><span>Primary unbounded</span></button>
<button class="button button--secondary-unbounded" type="button"><span>Secondary unbounded</span></button>
```


### Sizes

![](/content/design/sizes.png)

```html
<button class="button button--achromic button--small" type="button"><span>Small</span></button>
<button class="button button--achromic button--medium" type="button"><span>Medium</span></button>
<button class="button button--achromic button--large" type="button"><span>Large</span></button>
```

### States

![](/content/design/states.png)

```html
<button class="button button--achromic button--active" type="button"><span>Active</span></button>
<button class="button button--achromic disabled" type="button"><span>Disabled</span></button>
```

### Iconified

![](/content/design/iconified.png)

```html
<button class="button button--achromic button--text-hidden" type="button"><i class="oam-ds-icon-clock"></i><span>Hidden text</span></button>
<button class="button button--achromic" type="button"><i class="oam-ds-icon-clock"></i> <span>Visible text</span></button>
<button class="button button--achromic button--icon" type="button"></i><span>Pseudo-element</span></button>

```


### Groups

![](/content/design/groups.png)

```html
<div class="button-group button-group--horizontal" role="group" aria-label="...">
  <button class="button button--achromic button--active" type="button"><span>Left</span></button>
  <button class="button button--achromic" type="button"><span>Middle</span></button>
  <button class="button button--achromic" type="button"><span>Right</span></button>
</div>

<div class="button-group button-group--large button-group--horizontal">
  <label class="button button--achromic button--active" for="option-1">
    <input type="checkbox" id="option-1" checked=""> CB1 (pre-checked)
  </label>
  <label class="button button--achromic" for="option-2">
    <input type="checkbox" id="option-2"> CB2
  </label>
  <label class="button button--achromic" for="option-3">
    <input type="checkbox" id="option-3"> CB3
  </label>
</div>

<div class="button-group button-group--vertical" role="group" aria-label="...">
  <button class="button button--achromic" type="button"><span>Top</span></button>
  <button class="button button--achromic" type="button"><span>Middle</span></button>
  <button class="button button--achromic" type="button"><span>Bottom</span></button>
</div>

```

## Forms

### Examples

![](/content/design/forms-example.png)

```html
<form class="form">
  <fieldset class="form__fieldset">
    <legend class="form__legend">Fieldset legend 1</legend>
    <div class="form__group">
      <label class="form__label" for="form-name">Input text</label>
      <input type="text" class="form__control form__control--medium" id="form-name" name="form-name" placeholder="This is a placeholder" />
    </div>
    <div class="form__group">
      <label class="form__label" for="form-email">Input email</label>
      <input type="email" class="form__control form__control--medium" id="form-email" name="form-email" placeholder="This is a placeholder" />
      <div class="form__help">
        <p>This is some help text.</p>
      </div>
    </div>
    <div class="form__group">
      <label class="form__label">Checkboxes</label>
      <label class="form__option">
        <input type="checkbox" name="form-checkbox" id="form-checkbox-1" value="Checkbox 1" /> Checkbox 1
      </label>
      <label class="form__option">
        <input type="checkbox" name="form-checkbox" value="form-checkbox-2" /> Checkbox 2
      </label>
      <label class="form__option">
        <input type="checkbox" name="form-checkbox" value="form-checkbox-3" /> Checkbox 3
      </label>
    </div>
  </fieldset>
  <fieldset class="form__fieldset">
    <legend class="form__legend">Fieldset legend 2</legend>
    <div class="form__group">
      <label class="form__label" for="form-select-1">Select</label>
      <select class="form__control form__control--medium" id="form-select-1">
        <option>Option 1</option>
        <option>Option 2</option>
        <option>Option 3</option>
        <option>Option 4</option>
      </select>
    </div>
    <div class="form__group">
      <label class="form__label" for="form-file-1">File input</label>
      <input type="file" class="form__control" id="form-file-1" />
    </div>
    <div class="form__group">
      <label class="form__label" for="form-textarea-1">Textarea</label>
      <textarea class="form__control" id="form-textarea-1" rows="4" placeholder="This is a placeholder"></textarea>
    </div>
    <div class="form__group">
      <label class="form__label">Radios (inline)</label>
      <label class="form__option form__option--inline">
        <input type="radio" name="form-radio" id="form-radio-1" value="Radio 1" checked /> Radio 1
      </label>
      <label class="form__option form__option--inline">
        <input type="radio" name="form-radio" id="form-radio-2" value="Radio 2" /> Radio 2
      </label>
    </div>
  </fieldset>
</form>

```

### Control sizes

![](/content/design/form-control-sizes.png)

```html
<form class="form">
  <div class="form__group">
    <label class="form__label" for="form-input-1">Small</label>
    <input type="text" class="form__control form__control--small" id="form-input-1" placeholder="This is a placeholder" />
  </div>
  <div class="form__group">
    <label class="form__label" for="form-input-2">Medium</label>
    <input type="text" class="form__control form__control--medium" id="form-input-2" placeholder="This is a placeholder" />
  </div>
  <div class="form__group">
    <label class="form__label" for="form-input-3">Large</label>
    <input type="text" class="form__control form__control--large" id="form-input-3" placeholder="This is a placeholder" />
  </div>
  <div class="form__group">
    <label class="form__label" for="form-input-4">XLarge</label>
    <input type="text" class="form__control form__control--xlarge" id="form-input-4" placeholder="This is a placeholder" />
  </div>
</form>

```

### Custom options (radios and checkboxes)

![](/content/design/form-custom.png)

```html
<form class="form">
  <div class="form__group">
    <label class="form__label">Checkboxes</label>
    <label class="form__option form__option--custom-checkbox">
      <input type="checkbox" name="form-custom-checkbox" id="form-custom-checkbox-1" value="Checkbox 1" />
      <span class="form__option__text">Checkbox 1</span>
      <span class="form__option__ui"></span>
    </label>
    <label class="form__option form__option--custom-checkbox">
      <input type="checkbox" name="form-custom-checkbox" value="form-custom-checkbox-2" />
      <span class="form__option__text">Checkbox 2</span>
      <span class="form__option__ui"></span>
    </label>
    <label class="form__option form__option--custom-checkbox">
      <input type="checkbox" name="form-custom-checkbox" value="form-custom-checkbox-3" />
      <span class="form__option__text">Checkbox 3</span>
      <span class="form__option__ui"></span>
    </label>
  </div>
  <div class="form__group">
    <label class="form__label">Radios</label>
    <label class="form__option form__option--custom-radio">
      <input type="radio" name="form-custom-radio" id="form-custom-radio-1" value="Radio 1" checked />
      <span class="form__option__text">Radio 1</span>
      <span class="form__option__ui"></span>
    </label>
    <label class="form__option form__option--custom-radio">
      <input type="radio" name="form-custom-radio" id="form-custom-radio-2" value="Radio 2" />
      <span class="form__option__text">Radio 2</span>
      <span class="form__option__ui"></span>
    </label>
  </div>
</form>

```

### Input groups

![](/content/design/form-input-groups.png)

```html
<form class="form">
  <div class="form__group">
    <label class="form__label" for="form-input-5">Input group</label>
    <div class="form__input-group">
      <input type="text" class="form__control form__control--medium" id="form-input-5" placeholder="This is a placeholder">
      <span class="form__input-group-button"><button type="submit" class="button button--achromic button--text-hidden button--medium button--example-icon"><span>Button</span></button></span>
    </div>
  </div>

  <div class="form__group">
    <label class="form__label" for="form-input-6">Input group</label>
    <div class="form__input-group">
      <span class="form__input-group-button"><button type="submit" class="button button--achromic button--text-hidden button--medium button--example-icon"><span>Button</span></button></span>
      <input type="text" class="form__control form__control--medium" id="form-input-6" placeholder="Search location">
    </div>
  </div>
</form>
```

## Drops

### Examples

![](/content/design/dropdown-example.png)

```html
<div class="drop drop--down drop--align-left drop--open">
  <button class="button button--achromic drop__toggle" type="button"><span>Toggle</span></button>
  <div class="drop__content">
    <ul class="drop__menu" role="menu">
      <li><a href="#" title="This is Item 1a" class="drop__menu-item">Item 1a</a></li>
      <li><a href="#" title="This is Item 2a" class="drop__menu-item">Item 2a</a></li>
    </ul>
    <ul class="drop__menu" role="menu">
      <li><a href="#" title="This is Item 1b" class="drop__menu-item">Item 1b</a></li>
      <li><a href="#" title="This is Item 2b" class="drop__menu-item">Item 2b</a></li>
    </ul>      
    <div class="drop__inset">
      <p>This is a drop inset.</p>
    </div>          
  </div>
</div>

<div class="drop drop--down drop--align-left drop--open">
  <button class="button button--achromic drop__toggle" type="button"><span>Toggle</span></button>
  <div class="drop__content">
    <h6 class="drop__title">This is a title</h6>
    <ul class="drop__menu" role="menu">
      <li><a href="#" title="This is Item 1a" class="drop__menu-item">Item 1a</a></li>
      <li><a href="#" title="This is Item 2a" class="drop__menu-item">Item 2a</a></li>
    </ul>
    <div class="drop__inset">
      <p>This is a drop inset.</p>
    </div> 
    <ul class="drop__menu" role="menu">
      <li><a href="#" title="This is Item 1b" class="drop__menu-item">Item 1b</a></li>
      <li><a href="#" title="This is Item 2b" class="drop__menu-item">Item 2b</a></li>
    </ul>
  </div>
</div>

<div class="drop drop--down drop--align-left drop--open">
  <button class="button button--achromic drop__toggle" type="button"><span>Toggle</span></button>
  <div class="drop__content">
    <div class="drop__inset">
      <p>This is a drop inset.</p>
    </div> 
    <ul class="drop__menu" role="menu">
      <li><a href="#" title="This is Item 1a" class="drop__menu-item">Item 1a</a></li>
      <li><a href="#" title="This is Item 2a" class="drop__menu-item">Item 2a</a></li>
    </ul>
  </div>
</div>
```

### Iconified and selectable menus

![](/content/design/iconified-dropdown.png)

```html
<div class="drop drop--down drop--align-left drop--open">
  <button class="button button--achromic drop__toggle drop__toggle--caret" type="button"><span>Toggle</span></button>
  <div class="drop__content">
    <h6 class="drop__title">This is a title</h6>
    <ul class="drop__menu drop__menu--iconified" role="menu">
      <li><a href="#" title="This is Item 1a" class="drop__menu-item"><i class="oam-ds-icon-pencil"></i>Edit</a></li>
      <li><a href="#" title="This is Item 2a" class="drop__menu-item drop__menu-item--example-icon">Download</a></li>
    </ul>
    <ul class="drop__menu drop__menu--iconified" role="menu">
      <li><a href="#" title="This is Item 1a" class="drop__menu-item delete"><i class="oam-ds-icon-trash-bin"></i>Delete</a></li>
    </ul>
  </div>
</div>

<div class="drop drop--down drop--align-left drop--open">
  <button class="button button--achromic drop__toggle drop__toggle--caret" type="button"><span>Toggle</span></button>
  <div class="drop__content">
    <h6 class="drop__title">This is a title</h6>
    <ul class="drop__menu drop__menu--select" role="menu">
      <li><a href="#" title="This is Item 1b" class="drop__menu-item drop__menu-item--active">Item 1b</a></li>
      <li><a href="#" title="This is Item 2b" class="drop__menu-item">Item 2b</a></li>
      <li><a href="#" title="This is Item 3b" class="drop__menu-item">Item 3b</a></li>
    </ul>
  </div>
</div>
```

### React examples

The `oam-design-system` also provides some [React](https://facebook.github.io/react/) ready-made components that can be used for the interactive pieces.

```html
import { Dropdown } from 'oam-design-system';

// Minimum properties are:
// triggerText and triggerClassName
<Dropdown
  triggerClassName='button button--achromic'
  triggerText='Toggle' >

  Content can be anything.
</Dropdown>

// Example with all properties
// Elements availale: a / button (default)
// Directions available: up / down (default)
// Aligments available: left / center (default) / right
<Dropdown
  className='drop__content--special'
  triggerElement='a'
  triggerClassName='button button--achromic drop__toggle--caret'
  triggerTitle='Show/hide options'
  triggerText='Toggle'
  direction='up'
  aligment='left' >

  Content can be anything.
</Dropdown>
```

## Panels

![](/content/design/panels.png)

```html
<section class="panel">
  <header class="panel__header">
    <div class="panel__headline">
      <h1 class="panel__title">Panel title</h1>
      <div class="panel__subtitle">Panel subtitle</div>
    </div>
  </header>
  <div class="panel__body">
    <div class="panel__body-inner">
      <p>This is the panel body.</p>
    </div>
  </div>
  <footer class="panel__footer"></footer>
</section>
```

### Custom scrollbars

Whenever the content is too big for its container we use a custom scrollbar. This allows for better integration with the OAM style.  
The scroll behavior is provided by [reactScrollbar](https://github.com/souhe/reactScrollbar), but since it's not part of the `oam-design-system` it needs to be manually installed:

```
npm install react-scrollbar --save
```

The following example is specific to panels but with minor tweaks it can be used anywhere.


![](/content/design/react-scrollbar.png)

```html
// We include custom styling to match the OAM style, therefore
// react-scrollbar needs to be imported without stock styles.
import ScrollArea from 'react-scrollbar/dist/no-css';

<section className='panel'>
  <header className='panel__header'>
    <div className='panel__headline'>
    <h1 className='panel__title'>Panel title lorem ipsum dolor sit amet</h1>
      <div className='panel__subtitle'>Panel subtitle</div>
    </div>
    <div className='panel__meta-actions'>
      <button className='panel__button-dismiss' title='Dismiss panel'><span>Dismiss</span></button>
    </div>
  </header>
    <ScrollArea
      speed={1.6}
      className='panel__body'
      contentClassName='panel__body-inner'
      smoothScrolling={true}
      horizontal={false} >

      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium numquam officiis aliquid harum similique fugit molestiae sequi, corrupti. Quo accusantium, soluta corporis molestiae, eos suscipit expedita aspernatur rerum ad ea!</p>
    </ScrollArea>
  <footer className='panel__footer'></footer>
</section>
```

## Alerts

### Block

![](/content/design/alert-block.png)

```html
<div class="alert alert--success" role="alert">
  <button class="alert__button-dismiss" title="Dismiss alert"><span>Dismiss</span></button>
  <p><strong>Success:</strong> This is a success alert message.</p>
</div>

<div class="alert alert--info" role="alert">
  <button class="alert__button-dismiss" title="Dismiss alert"><span>Dismiss</span></button>
  <p><strong>Info:</strong> This is an info alert message.</p>
</div>

<div class="alert alert--warning" role="alert">
  <button class="alert__button-dismiss" title="Dismiss alert"><span>Dismiss</span></button>
  <p><strong>Warning:</strong> This is a warning alert message.</p>
</div>

<div class="alert alert--danger" role="alert">
  <button class="alert__button-dismiss" title="Dismiss alert"><span>Dismiss</span></button>
  <p><strong>Danger:</strong> This is a danger alert message.</p>
</div>
```

### Popover

![](/content/design/popover.png)
```html
<div class="alert alert--popover alert--danger" role="alert">
  <button class="alert__button-dismiss" title="Dismiss alert"><span>Dismiss</span></button>
  <p><strong>Danger:</strong> This is a danger alert message. Popover style!</p>
</div>
```

## Modal

### Static example

![](/content/design/modal.png)

```html
<section class="modal">
  <div class="modal__inner">
    <header class="modal__header">
      <div class="modal__headline">
        <p class="modal__subtitle">Modal subtitle</p>
        <h1 class="modal__title">Modal title</h1>
      </div>
    </header>
    <div class="modal__body">
      <p>This is a paragraph.</p>
    </div>
    <footer class="modal__footer">
      <button class="button button--achromic" type="button"><span>Cancel</span></button>
      <button class="button button--base" type="button"><span>Save</span></button>
    </footer>
  </div>
  <button class="modal__button-dismiss" title="Close"><span>Dismiss</span></button>
</section>
```

### React example

A modal must always have a `ModalHeader` and a `ModalBody`. The `ModalFooter` is entirely optional.  

The visibility of the modal is controlled by the `revealed` property. The modal does not implement any mechanism to toggle its state. It is up to you to handle the click (`onCloseClick`) and properly change the `revealed` property.

```js

import OAM from 'oam-design-system';
var { Modal, ModalHeader, ModalBody, ModalFooter } = OAM.Modal;

  <Modal
    id='modal-showcase'
    className='modal--large'
    onCloseClick={this.closeModal}
    revealed={this.state.open} >

    <ModalHeader>
      <div className='modal__headline'>
        <p className='modal__subtitle'>Excerpt</p>
        <h1 className='modal__title'>The Last Question</h1>
      </div>
    </ModalHeader>
    <ModalBody>
      <div className='prose'>
        <p>All other questions had been answered, and until this last question was answered also, AC might not release his consciousness.</p>
        <p>All collected data had come to a final end. Nothing was left to be collected. But all collected data had yet to be completely correlated and put together in all possible relationships.</p>
        <p>A timeless interval was spent in doing that.</p>
      </div>
    </ModalBody>
    <ModalFooter>
      <cite><a href='http://multivax.com/last_question.html' title='Open The Last Question'>The Last Question</a>, Isaac Asimov 1956</cite>
    </ModalFooter>
  </Modal>

```
