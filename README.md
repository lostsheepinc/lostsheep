## Welcome to LostSheep

Data is valuable, and missing data poses a significant risk to your business. LostSheep discovers and explains your data quality problems, helping you to resolve them faster than ever before.

## LostSheep in action:

A drinks company carried out some market research with the hope of identifying peoples favourite spirit, ending up with the following dataset:

`data = `

Name|Age|Country|Favourite Spirit
----|:---:|:---:|:----:
Jack|43|USA|Whiskey
John|14|UK|
Jane|37|UK|Gin
Jill|20|USA|
Josh|19|UK|Vodka
...|...|...|...

Their survey results contain missing data, and they are keen to understand the reasons behind this.

With LostSheep, this can be done in just a couple of lines:

```python
>>> from lostsheep import LostSheep
>>> LostSheep(data).explain('Favourite Spirit')
['Country = USA and Age < 21', 'Country = UK and Age < 18']
```

The company now understand that the survey was not answered by people below the legal drinking age in their country. 

This example is trivial as there are only a few columns, but with hundreds of columns and numerous complex dependencies in the data, LostSheep becomes incredibly useful.


<form method="POST" action="https://formspree.io/lostsheepinc@gmail.com">
  <input type="email" name="email" placeholder="Your email">
  <textarea name="message" placeholder="Test Message"></textarea>
  <button type="submit">Send Test</button>
</form>
