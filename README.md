# Project Title

This is an exercise where we create a secret word that will show random stuff on the screen, based on the 30 days Javascript challenge.

## Getting Started

Type daniel on the screen.

## Demo

## [Key Sequence](https://danielgarciaguillen.github.io/keysequence/)



## Learnings

* How to log the key that you press, push it to an array and check if contains the secret code:

```
const pressed = [];
const secretCode = 'daniel';
window.addEventListener('keyup', (e) =>{
    console.log(e);
    pressed.push(e.key);
    pressed.splice(-secretCode.length -1, pressed.length - secretCode.length);

    if(pressed.join('').includes(secretCode)){
        console.log("DING DING");
        cornify_add();
    }
    console.log(pressed);
})
```


## Built With

* Vanilla Javascript
* Css
* Html
