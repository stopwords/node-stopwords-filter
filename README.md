# node-stopwords-filter

Stopwords filter for Nodejs, Javascript

`Vietnamese` and `English` database supported.

# Install
```
npm install node-stopwords-filter
```

# Example 

```js
var StopwordsFilter = require('node-stopwords-filter');
var f = new StopwordsFilter();

var input = "a whole new category is good for me";
console.log(f.filter(input));
// => [ 'category', 'good' ]

// Output as string
console.log(f.filter(input, 'string'));
// => 'category good'
```

# API

### Set stopwords language

```js
var StopwordsFilter = require('node-stopwords-filter');
var f = new StopwordsFilter({
	lang: 'vi'
});

// Or
f.setLanguage('vi');
```

# Test

```sh
npm test
```

# TODO

* Tokenizer string for Vietnamese (See: https://github.com/duyetdev/node-vntokenizer)

# How to contribute
1. Fork the project on Github
2. Create a topic branch for your changes
3. Ensure that you provide documentation and test coverage for your changes (patches won’t be accepted without)
4. Create a pull request on Github (these are also a great place to start a conversation around a patch as early as possible)

# License
MIT License

Copyright (c) 2015 Van-Duyet Le

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
