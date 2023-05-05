# Frontend Mentor - Product preview card component solution

## Edit

- I took the advice and turned: font, margin, and padding to rem's. I switch my div .container to main and I switched my width and height. In body to min-height: 100vh
  and turned width to max-width in .container.

### The challenge

- [View the optimal layout depending on their device's screen size](#Issues)
  - I did the main screen alright it was when I went to make the mobile version I realized I should have tackled the margin-top differently by using gap or something. I had to reset all my margins which seemed a bit overdoing it.

### Screenshot

![desktop version](/images/screen-shot-desktop.png)

![mobile version](/images/screen-shot-mobile.png)

### What I learned

I don't know if you call it learning as more knowing what I am doing can be done cleaner. I only say that because I was repeating a bit of code knowing that there's got to be a better way. When I went to do the mobile version using @media I then discovered what I mentioned doubled. I had to keep resetting my margin-top in multiple classes which I know with time I will learn to consolidate my code to be more reusable, but for now, I am happy to at least get it to work.
I did learn the picture element. That one was pretty handy to switch from mobile to desktop.
The .svg in the button I don't understand what happened but when I put it in as an image it blew up in size then when I tried to set the size it inverted it so it was facing the other direction and a little deformed. What I did I know is sloppy, but again for now I got it working. Just something else for me to look into.

- picture element

```html
<picture>
  <source
    srcset="./images/image-product-mobile.jpg"
    media="(max-width: 600px)"
  />
  <img src="./images/image-product-desktop.jpg" alt="perfume" />
</picture>
```

- my .svg inserted into the button. Not too clean looking

```html
<button>
  <svg width="15" height="16" xmlns="http://www.w3.org/2000/svg">
    <path
      d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z"
      fill="#FFF"
    /></svg
  ><span>Add to Cart</span>
</button>
}
```

### Useful resources

- [resource](https://www.duckduckgo.com) - Need I say more
