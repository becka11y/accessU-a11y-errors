---?color=#36173A
## Link Text

Note: 2.4.4 Link Text (in-context) Level A
---
@snap[north span-80]
## Passable (in-context) Link Text
@snapend

@snap[south span-80]
![alt=screen shot showing use of here link text within a paragraph](techniques/link-text/img/link-purpose-in-context.png)
@snapend

---
@snap[north span-80]
## Better Link Text
@snapend

@snap[south span-80]
![alt=screen shot showing use of here link text within a paragraph](techniques/link-text/img/link-purpose-in-context-improved.png)
@snapend

---
@snap[north span-80]
## Why Link Text Matters
@snapend

@snap[midpoint span-50]
![alt=screen shot of VoiceOver list of links](techniques/link-text/img/links-list.png)
@snapend

---
@snap[north span-80]
## The Origin of the List
@snapend

@snap[midpoint span-60]
![alt=screen shot of tour dates for a band with links that just say Tickets](techniques/link-text/img/links-full-view.png)
@snapend

Note: Note the low color contrast of white on blue. Think about all of Click here or Read More links you see on sites

live example:  https://thelumineers.com/tour-dates/ - repeating tickets. Can fix with aria-label or add date to "button" (really a link) text. Also opens in new window when follow.
---
@snap[north span-80]
## Another Link Text Example
@snapend


![alt=screen shot with various loan options, each with a Apply Now and Learn More link](techniques/link-text/img/link-text-loan-info.png)

Note: These apply now and learn more links have aria-labels that distinguish them
---
@snap[north span-80]
## Example Zoomed to 400%
@snapend

![alt=screen shot with various loan options, each with a Apply Now and Learn More link](techniques/link-text/img/link-text-loan-info-zoom400.png)

Note: affects people using screen magnification and/or speech input
---
@snap[north span-80]
## How to fix Vague Link Text
@snapend

@snap[west span-100]
@ul[](false)
- Add more detail to the visible label
  - include the date or location
  - incorporate surrounding text that adds context
- Add an aria-label - only helps screen readers
@ulend
@snapend

@snap[south-west span-100]
```html zoom-15 code-wrap
 <a href="url-to-Visa-apply" aria-label="Visa® Platinum Credit Card APPLY NOW">APPLY NOW</a>
```
@snapend

Note: live example:  https://thelumineers.com/tour-dates/ - repeating tickets. Can fix with aria-label or add date to "button" (really a link) text. Also opens in new window when follow.
