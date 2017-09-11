### Slide-to-Tab--Jquery
Click on an anchor tab to slide to a section on the same page

```html 
Anchor tag to be clicked (to go to the section we want to check out)-

<a style="color:blue;font-size:25px" id="port" href="#">Portfolio</a> | 
```
```html 
Anchor tag of the section we want to check out-

<a name="port1"/><h2 style="font-family:'Charlesworth';color:red;font-size:25px;
text-decoration:underline">PORTFOLIO</h2>
```
```javascript
Jquery for the slide function (using animate and scroll)- 

<script type="text/javascript">
function scrollToAnchor(aid){
    var aTag = $("a[name='"+ aid +"']");
    $('html,body').animate({scrollTop: aTag.offset().top},'slow');
}

$("#port").click(function() {
   scrollToAnchor('port1');
});
```

