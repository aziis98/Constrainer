# Constrainer

**Bad writing capabilities ahead**
This is a sass/css framework based on **absolute positioning** of elements and easy centering with **felxbox**es

## Reference

By convention classes like `.content-` affect the layout of the children elements while other classes like `.center-h` affect the element itself

### All elements

All elements use by default absolute positioning, border-box box-sizing, margin 0, padding 0 and text align center

### .fillpage

Makes the element fill the whole page

### .content-flow-h

Elements within flow horizontally and are centered on the horizontal mid line of the container

**.content-flow-hv**

Centers the elements also vertically

### .content-flow-v

Elements within flow vertically and are centered on the vertival mid line of the container

**.content-flow-vh**

Centers the elements also horizontally

## Supposed Usage

Example 1:

HTML:
```html
    <div class="fill-page">
        <div id="left-box">
            Some Text
            <div id="centered" class="center-x center-y">
                Centered!
            </div>
        </div>
        <div id="right-box" class="content-flow-v">
            <div class="element"></div>
            <div class="element"></div>
            <div class="element"></div>
        </div>
    </div>
```

```sass
    #left-box
        left: 0
        top: 0
        bottom: 0
        width: 400
```