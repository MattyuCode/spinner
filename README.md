```html 
<div class="spinner">
  <div class="loader"><span>{</span>/<span>}</span></div>
</div>
```

```css
 .spinner {
        /* height: 100%; */
        height: 100vh;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }


    .loader {
        opacity: 0.8;
        color: hsl(220deg 96% 49%);
        font-size: 20vh;
        font-weight: bold;
        font-family: Consolas, Menlo, Monaco, monospace;
    }

    .loader span:nth-child(odd) {
        animation-delay: 0.5s;
    }


    .loader span {
        display: inline-block;
        animation: pulse 0.5s alternate infinite ease-in-out;
    }

    @keyframes pulse {
        from {
            /* color: rgb(67, 126, 243); */
            font-size: 19vh;

        }

        to {
            color: rgb(67, 126, 243);
        }
    }
