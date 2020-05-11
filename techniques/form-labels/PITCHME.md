---?color=#36173A

## Form Labels

---
@snap[north span-80]
## VoiceOver Poor Label Example
@snapend

@snap[midpoint span-80 fragment]
![alt=screen shot of VO panel with focus on empty field](techniques/form-labels/img/form-label-poor-VO.png)
@snapend

Note: Run the VO live example before exposing the fragment!
 https://myaccount.palmergasco.com/become-customer.php
Form has no programmatically associated label, no programmatic indication of required, poor label text
---
@snap[north span-80]
## Poor Label Example
@snapend

@snap[west span-40]
![alt=screen shot of registration form](techniques/form-labels/img/form-label-poor.png)
@snapend

@snap[east span-40]
![alt=screen shot of registration form zoomed](techniques/form-labels/img/form-label-zoomed.png)
@snapend

---
@snap[north span-80]
## Form Label Requirements
@snapend

@snap[midpoint  span-90]
@ul
- Labels must exist
- Labels must be descriptive
- Labels must be programmatically associated with control
@ulend
@snapend

---
@snap[north span-80]
## Label Code example
@snapend

@snap[west span-90]
Screen reader hears the "star"

``` html zoom-15 code-wrap
  < label for="fname">
       *First Name:
  </label>
  <input id="fname" type="text" required>
```

@snapend

@snap[south-east span-70 fragment]
does hear "required"
@snapend


---
@snap[north span-80]
## Label Code example 2
@snapend

@snap[west span-100]
Screen reader does **NOT** hear the "star"

``` html zoom-15 code-wrap
  < label for="fname">
       <span aria-hidden="true">*</span>
       First Name:
  </label>
  <input id="fname" type="text" required>
```
@snapend
@snap[south-east span-70 fragment]
does hear "required"
@snapend

---
@snap[north span-80]
## Another Label Technique
@snapend

@snap[midpoint span-80]
[Avoid Placeholder Text by Animating Form Labels](https://knowbility.org/blog/2019/animating-form-labels/)
@snapend