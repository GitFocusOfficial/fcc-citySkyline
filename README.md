# Learn CSS Variables by Building a City Skyline

CSS variables help you organize your styles and reuse them.

In this course, you'll build a city skyline. You'll learn how to configure CSS variables so you can reuse them whenever you want.

## Step 1

Welcome to the CSS Variables Skyline project! Start by adding the `!DOCTYPE html` declaration at the top of the document so the browser knows what type of document it's reading.

## Step 2

Add opening and closing `html` tags below the `DOCTYPE` so you have a place to start putting some code. Be sure to set the language to English.

## Step 3

Next, add opening and closing `head` and `body` tags within the `html` element.

## Step 4

Within the `head`, nest a `meta` element with a `charset` of `UTF-8`, a `title` element with a title of `City Skyline`, and a `link` element that links your `styles.css` file.

## Step 5

In CSS, you can target everything with an asterisk. Add a border to everything by using the `*` selector, and giving it a `border` of `1px solid black`. This is a trick that helps visualize where elements are and their size. You will remove this later.

## Step 6

Also add a `box-sizing` of `border-box` to everything. This will make it so the border you added doesn't add any size to your elements.

## Step 7

You can see the `body` (it's the inner-most box on your page); the box around it is the `html` element. Make your `body` fill the whole viewport by giving it a `height` of `100vh`. Remove the default `margin` from the `body` by setting the `margin` to `0`. Finally, set the `overflow` property to `hidden` to hide any scroll bars that appear when something extends past the viewport.

## Step 8

Create a div element in the `body` with a class of `background-buildings`. This will be a container for a group of buildings.

## Step 9

Give your `.background-buildings` element a `width` and `height` of `100%` to make it the full width and height of its parent, the `body`.

## Step 10

Nest a `div` with a class of `bb1` in the background buildings container. Open your `styles.css` file, and give `.bb1` a `width` of `10%` and `height` of `70%`. "bb" stands for "background building", this will be your first building.

## Step 11

Nest four `div` elements in the `.bb1` container. Give them the classes `bb1a`, `bb1b`, `bb1c`, and `bb1d` in that order. This building will have four sections.

## Step 12

Give the parts of your building `width` and `height` properties with these values: `70%` and `10%` to `.bb1a`, `80%` and `10%` to `.bb1b`, `90%` and `10%` to `.bb1c`, and `100%` and `70%` to `.bb1d`. Remember that these percentages are relative to the parent and note that the heights will add up to 100% - vertically filling the container.

## Step 13

Center the parts of your building by turning the `.bb1` element into a flexbox parent. Use the `flex-direction` and `align-items` properties to center the children.

## Step 14

Now you have something that is resembling a building. You are ready to create your first variable. Variable declarations begin with two dashes (`-`) and are given a name and a value like this: `--variable-name: value;`. In the rule for the `bb1` class, create a variable named `--building-color1` and give it a value of `#999`.

## Step 15

To use a variable, put the variable name in parentheses with `var` in front of them like this: `var(--variable-name)`. Whatever value you gave the variable will be applied to whatever property you use it on.

Add the variable `--building-color1` you created in the previous step as the value of the `background-color` property of the `.bb1a` class.

## Step 16

Use the same variable as the `background-color` of the `.bb1b`, `.bb1c`, and `.bb1d` classes to fill in the rest of the building.

## Step 17

Change the value of your variable from `#999` to `#aa80ff` and you can see how it gets applied everywhere you used the variable. This is the main advantage of using variables, being able to quickly change many values in your stylesheet by just changing the value of a variable.

## Step 18

Your first building looks pretty good now. Nest three new `div` elements in the `.background-buildings` container and give them the classes of `bb2`, `bb3`, and `bb4` in that order. These will be three more buildings for the background.

## Step 19

Give the new buildings `width` and `height` properties of: `10%` and `50%` for `.bb2`, `10%` and `55%` for `.bb3`, and `11%` and `58%` for `.bb4`. You will be using almost all percent based units and some flexbox for this project, so everything will be completely responsive.

## Step 20

The buildings are currently stacked on top of each other. Align the buildings by turning the `.background-buildings` element into a flexbox parent. Use the `align-items` and `justify-content` properties to evenly space the buildings across the bottom of the element.

## Step 21

The buildings are too spaced out. Squeeze them together by adding two empty `div` elements to the top of the `.background-buildings` element, two more at the bottom of it, and one more in between `.bb3` and `.bb4`. These will be added as evenly-spaced elements across the container, effectively moving the buildings closer to the center.