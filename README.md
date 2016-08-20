# D3-Population-Pyramid
D3 Population Pyramid in D3 v4. You'll need only popPyramid.js and D3 for your own implementation. The easiest use is to include this in your header:

`  <script src="popPyramid.js"></script>`

And include something like this in your body:

```
<script>
  // data must be in a format with age, male, and female in each object
  var exampleData = [{ age: '0-9', male: 10, female: 12 }, { age: '10-19',
  male: 14, female: 15 }, { age: '20-29', male: 15, female: 18 }, { age:
    '30-39', male: 18, female: 18 }, { age: '40-49', male: 21, female: 22 }, {
      age: '50-59', male: 19, female: 24 }, { age: '60-69', male: 15, female: 14 }, {
        age: '70-79', male: 8, female: 10 }, { age: '80-89', male: 4, female: 5 }, {
          age: '90+', male: 2, female: 3 }];

  pyramidBuilder(exampleData, '#pyramid', 400, 500);
</script>
  ```

The chart (with default css) looks something like this:

![alt text](https://raw.github.com/doylek/D3-Population-Pyramid/screenshot/screenshot.png "example screenshot")


# Options

| Name | Type | Default| Optional |   Notes  |
|------|------|--------|----------|----------|
| data | JSON | N/A | N           | Needs age, male, and female properties. <br /> Example: [{ age: '0-50', male: 4500, female: 4500 }, { age: '51-99+',male: 5000, female: 5000 }]|
| target | string | N/A | N       | Uses D3's select() function. Examples: '#pyramid', 'body' |
| height | numeric | 400 | Y      |          |
| width |  numeric  | 400 | Y     |           |
| style | JSON    | see below | Y | Example: {leftBarColor: '#00ffaa', rightBarColor: '#ffaa00', tooltipBG: '#333', tooltipColor: 'white'} |
| style.leftBarColor | string (hex) | '#6c9dc6' | Y | Input color will be automatically lightened for :hover css |
| style.rightBarColor | string (hex) | '#de5454' | Y  | Input color will be automatically lightened for :hover css|
| style.tooltipBG |   string (hex) | '#fefefe' | Y  | Uses CSS background property, so you could use more than just a color value. |
| style.tooltipColor |   string (hex) | 'black' | Y  |  Controls CSS color property for tooltip  |
