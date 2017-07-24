# Make Your Own Mondrian-Style Painting with Code
Use HTML and CSS to create a Mondrian-style painting

Modified from [Google Coder project](https://googlecreativelab.github.io/coder-projects/projects/mondrian/)

<img src="http://i.imgur.com/lETX0Is.jpg" width="400" alt="Mondrian-style Code Painting">

# Tutorial

## First Half
[First half](https://googlecreativelab.github.io/coder-projects/projects/mondrian/) will get you to here:

<img src="http://i.imgur.com/v4BJDcP.png" width="400" alt="Mondrian-style Code Painting">

## Second Half

### Step 10: Bottom Right Boxes (Blue and Yellow)
- Add a div for the bottom row:

```
<div id="bottom-row">
</div>
```
- Inside that div, let's add another div for the bottom right column. We want to start from the right, so we'll add the `right` class to it.

```
<div id="bottom-row">
  <div id="bottom-right-column" class="right">
  </div>
</div>
```

- Inside _that_ div, let's create a small box, add a small divider, and a second small box:
```
  <div id="bottom-right-column" class="right">
    <div class="small-box blue right"></div>
    <div id="divider-5" class="black right"></div>
    <div class="small-box yellow right"></div>
  </div>
```

Now we have a basic layout for the two small boxes on the bottom right! Let's style them!

- Let's give the `#bottom-right-column` element a height of 100px and a width of 40px.
```
#bottom-right-column {
  height: 100px;
  width: 40px;
}
```

- Now, let's give the `.small-box` class a width of 50px and a height of 45px:
```
.small-box {
  width: 50px;
  height: 45px;
}
```

- Next, let's style the divider:
```
#divider-5 {
  height: 10px;
  width: 50px;
}
```

- Finally, let's add a divider, named `divider-6`, to the left of the bottom right column:
```
<div id="bottom-right-column" class="right">
  <div class="small-box blue right"></div>
  <div id="divider-5" class="black right"></div>
  <div class="small-box yellow right"></div>
</div>

<div id="divider-6" class="right black"></div>
```

### Step 11: Bottom Middle Box
- *Inside* the `bottom-row` div, we're going to add a `bottom-middle-box` div:
```
<div id="divider-6" class="right black"></div>
        
<div id="bottom-middle-box" class="right"></div>
```

- Let's style the `bottom-middle-box` div! We're going to give it a height of 100px and a width of 240px.
```
#bottom-middle-box {
  height: 100px;
  width: 240px;
}
```

- Next, let's add a divider, `divider-4` to the left of that box, with the `.black` and `.right` classes assigned to it:
```
        <div id="bottom-middle-box" class="right"></div>
        <div id="divider-4" class="black right"></div>
```

- Let's style the divider we just added:
```
#divider-4 {
  height: 100px;
  width: 10px;
}
```

### Step 12: Bottom Left Box (Blue)
- Last box! Let's add a div for the `bottom-left-box`:
```
        <div id="divider-4" class="black right"></div>
        <div id="bottom-left-box" class="blue right"></div>
```

- Let's style `bottom-left-box`:
```
#bottom-left-box {
  width: 100px;
  height: 100px;
}
```

