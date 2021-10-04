# customjquery
similar like jquery

## Step1: Create a file named mylibrary.js and add below code
```javascript
const $ = (selector) => {
    let sthis = this;
    const self = {
        element: document.querySelector(selector),
        html: () => self.element,
        hide: () => {
            self.element.style.display = "none";
        }
    }
    return self
}
```

## Step2: usage
```javascript
<script src="assets/mylibrary.js"></script>
  <script>
    setTimeout( () => {
      $('h4').hide();
    }, 2000);
  </script>
```
