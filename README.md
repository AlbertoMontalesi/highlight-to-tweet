## Description

Highlight text and share it easily on twitter

Inspired by [this](https://webflow.com/website/Highlight-text-to-Tweet-it)

## Installation 

Install using `npm i highlight-to-tweet`

Import like this: `const highlight = require('highlight');`

And use like this:

```js
highlight({
    ...yoursettings
});
```

&nbsp;

## Settings

These are the allowed properties you can pass to override the default one
```js
 const settings = {
    cssClassess: string[], // extra classed to add to the container if you want to style it yourself
    minLength: number,
    maxLength: number,
    extra:string, // extra text to append to the tweet
    via: string, // your twitter handler
    popupArgs: string,
    callback: Function,
}
```

Default configuration:

```js
 const settings = {
    node: "<a href='#'>Tweet</a>",
    cssClassess: ['tweet-me'],
    minLength: 1,
    maxLength: 144 * 4,
    extra: '',
    via:null,
    popupArgs:'width=400,height=400,toolbar=0,location=0',
    callback: null,
}
```

## License

MIT License

Copyright (c) 2020 Alberto Montalesi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.