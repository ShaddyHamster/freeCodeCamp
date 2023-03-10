---
id: 56533eb9ac21ba0edf2244b7
title: Об'єднання рядків за допомогою оператора "плюс"
challengeType: 1
videoUrl: 'https://scrimba.com/c/cNpM8AN'
forumTopicId: 16802
dashedName: concatenating-strings-with-plus-operator
---

# --description--

В JavaScript, коли оператор `+` використовується зі значенням `String`, це називається оператором <dfn>об'єднання</dfn>. З рядків можна створити новий рядок, <dfn>об'єднавши</dfn> їх.

**Наприклад:**

```js
'My name is Alan,' + ' I concatenate.'
```

**Примітка:** Зверніть увагу на пробіли. Під час об'єднання між рядками відсутні пробіли, вам потрібно буде додати їх самостійно.

Наприклад:

```js
const ourStr = "I come first. " + "I come second.";
```

The string `I come first. I come second.` would be displayed in the console.
# --instructions--

Створіть `myStr` з рядків `This is the start.` й `This is the end.` за допомогою `+` оператору. Обов'язково використовуйте пробіл між двома рядками.

# --hints--

`myStr` should have a single space character between the two strings.

```js
assert(/start\. This/.test(myStr));
```

`myStr` should have a value of the string `This is the start. This is the end.`

```js
assert(myStr === 'This is the start. This is the end.');
```

You should use the `+` operator to build `myStr`.

```js
assert(code.match(/(["']).*\1\s*\+\s*(["']).*\2/g));
```

`myStr` should be created using the `const` keyword.

```js
assert(/const\s+myStr/.test(code));
```

You should assign the result to the `myStr` variable.

```js
assert(/myStr\s*=/.test(code));
```

# --seed--

## --after-user-code--

```js
(function(){
  if(typeof myStr === 'string') {
    return 'myStr = "' + myStr + '"';
  } else {
    return 'myStr is not a string';
  }
})();
```

## --seed-contents--

```js
const myStr = ""; // Change this line
```

# --solutions--

```js
const myStr = "This is the start. " + "This is the end.";
```
