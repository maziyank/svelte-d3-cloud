# svelte-d3-cloud

Svelte wrapper for [d3-cloud](https://github.com/jasondavies/d3-cloud)

## Installation

```js 
npm install svelte-d3-cloud
``` 
or
```js
yarn add svelte-d3-cloud
```

## Usage

```html

<script>
import WordCloud from "svelte-d3-cloud";

const words = [
    { text: "Halo", count: 100 },
    { text: "Dunia", count: 50 },
    { text: "Gaib", count: 75 },
  ];

</script>

<div>
  <WordCloud words={words}/>
</div>

```

## Props
| Property | Description             | Default Value |
|----------|-------------------------|---------------|
| words    | Array of object contains text and count value ``` [{text : "some", count: 10},...] ``` | undefined |
| width    | Set the word cloud canvas width  | 500           |
| height   | Set the word cloud canvas height | 500           |
| backgroundColor     | Set the canvas background color | '#fff'      |
| font     | Set the word font family | 'Impact'      |
| padding     | Set the padding of each text | 10     |
| scheme     | Set the word cloud text color scheme based on d3-scale-chromatic (schemeCategory10 , schemeAccent, schemeDark2, schemePaired, schemePastel1, schemePastel2, schemeSet1, schemeSet2, schemeSet3, schemeTableau10) | 'schemeTableau10'     |
| minRotate     | Set the minimum rotation of the text | 0     |
| maxRotate     | Set the maximum rotation of the text | 0     |
| maxFontSize     | Set the maximum font size of the text | 50     |
   
## Events

| Event | Description             |
|----------|-------------------------|
| on:click        | Listen to event when word is clicked | 
| on:mouseover    | Listen to event when word is hovered |
| on:mouseout     | Listen to event when mouse leave the word|
| on:mousemove    | Listen to event when mouse move inside the word |

