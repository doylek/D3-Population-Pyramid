# D3-Population-Pyramid
D3 Population Pyramid in D3 v4. You'll need only popPyramid.js for your own implementation. The easiest use is to include this in your header:

`  <script src="popPyramid.js"></script>`

And include something like this in your body:

```
<script>
  // data must be in a format with group, male, and female in each object
  var exampleData = [{ group: '0-9', male: 10, female: 12 }, { group: '10-19',
  male: 14, female: 15 }, { group: '20-29', male: 15, female: 18 }, { group:
    '30-39', male: 18, female: 18 }, { group: '40-49', male: 21, female: 22 }, {
      group: '50-59', male: 19, female: 24 }, { group: '60-69', male: 15, female: 14 }, {
        group: '70-79', male: 8, female: 10 }, { group: '80-89', male: 4, female: 5 }, {
          group: '90+', male: 2, female: 3 }];

  pyramidBuilder(exampleData, '#pyramid', 400, 500);
</script>
  ```
