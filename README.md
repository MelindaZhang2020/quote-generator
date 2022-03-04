# Zero to Mastery - Quote Generator (20 JavaScript Projects)

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

- Learn about API, how to fetch data from an API and manipulate it.

### Links

- Live Site URL: [Live site here](https://eager-archimedes-45170b.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Create a new resository on the command line:

```
echo "# quote-generator" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/MelindaZhang2020/quote-generator.git
git push -u origin main
```
[Hero Patterns](https://heropatterns.com/)

Useful shortcuts: Alt + z ---> word wrap for vscode

Good to know:
title attribute gives explanation to the element
```
 <button class="twitter-button" id="twitter" title="Tweet This!">
                <i class="fab fa-twitter"></i>
  </button>
```

New CSS tricks:
```
 width: auto;
```

```
font-style: italic;
```

```
margin: auto 10px;
```

async await 
```
// Get Quotes From API
async function getQuotes() {
  const apiUrl = 'https://type.fit/api/quotes';
  try{
    const response = await fetch(apiUrl);
    apiQuotes = await response.json();
    newQuote();
  } catch(err){
    // Catch Error Here
  }
}
```

Get a random index from an array
```
const quote = apiQuotes[Math.floor(Math.random()*apiQuotes.length)];
```

[Tweet button](https://developer.twitter.com/en/docs/twitter-for-websites/tweet-button/guides/web-intent)

```
function tweetQuote() {
  const twitterUrl = `https://twitter.com/intent/tweet?text=${quoteText.textContent} - ${authorText.textContent}`;
  window.open(twitterUrl, '_blank');
}
```

[Cors Error](https://medium.com/@dtkatz/3-ways-to-fix-the-cors-error-and-how-access-control-allow-origin-works-d97d55946d9)

## Author

- Website - [Melinda Zhang](https://www.melinda-zhang.com)

- Twitter - [@melindazhang4](https://www.twitter.com/melindazhang4)


