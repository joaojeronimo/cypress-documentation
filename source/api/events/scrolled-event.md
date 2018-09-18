---
title: scrolled
---

The `scrolled` event fires whenever **Cypress** is scrolling your application. This event is fired when Cypress is {% url 'waiting for and calculating actionability' interacting-with-elements %}. It will scroll to 'uncover' elements currently being covered. This event is extremely useful to debug why Cypress may think an element is not interactive.

# Environment

Event | {% url "Browser" catalog-of-events#Browser-Events %} | {% url "Background Process" background-process %}
--- | --- | ---
{% url `scrolled` scrolled-event %} | {% fa fa-check-circle green %} |

# Arguments

**{% fa fa-angle-right %} el** ***(Object)***

The element or `window` being scrolled

**{% fa fa-angle-right %} type** ***('element'|'window'|'container')***

The type of element being scrolled.

# Usage

```javascript
Cypress.on('scrolled', (elOrWindow, type) => {

})
```