# bxSlider

bxSlider 4.2.5 , http://bxslider.com



### Ư¡
* ������ ����.
* ����, ����, ���̵� ���
* �̹���, ����, html ������ ����
* ���� �żҵ�, �ݹ� API ����
* ���� ������: Firefox, Chrome, Safari, iOS, Android, IE7+



## ����


### Step 1: `js`, `css` ���� ��Ŭ���

```html
<!-- jQuery library (served from Google) -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<!-- bxSlider Javascript file -->
<script src="/js/jquery.bxslider.min.js"></script>
<!-- bxSlider CSS file -->
<link href="/lib/jquery.bxslider.css" rel="stylesheet" />
```

### Step 2: `HTML` ����


```html
<ul class="bxslider">
  <li><img src="/images/pic1.jpg" /></li>
  <li><img src="/images/pic2.jpg" /></li>
  <li><img src="/images/pic3.jpg" /></li>
  <li><img src="/images/pic4.jpg" /></li>
</ul>
```

### Step 3: bxSlider ȣ�� �� �ɼ�

```javascript
$(document).ready(function(){
    $('.bxslider').bxSlider( {
        mode: 'horizontal',// ���� ���� ���� �����̵�
        speed: 500,        // �̵� �ӵ��� ����
        pager: false,      // ���� ��ġ ����¡ ǥ�� ���� ����
        moveSlides: 1,     // �����̵� �̵��� ����
        slideWidth: 100,   // �����̵� �ʺ�
        minSlides: 4,      // �ּ� ���� ����
        maxSlides: 4,      // �ִ� ���� ����
        slideMargin: 5,    // �����̵尣�� ����
        auto: true,        // �ڵ� ���� ����
        autoHover: true,   // ���콺 ȣ���� ���� ����
        controls: false    // ���� ���� ��ư ���� ����
    });
});
```


## ���� �ɼ�

###General

**mode**
�����̵� ����
```
default: 'horizontal'
options: 'horizontal', 'vertical', 'fade'
```

**speed**
�����̵� ��ȯ �ð�(ms ����)
```
default: 500
options: integer
```

**slideMargin**
�� �����̵� ������ ����
```
default: 0
options: integer
```

**startSlide**
���� �����̵� �ε��� (zero-based)
```
default: 0
options: integer
```

**randomStart**
������ �����̵忡�� �����̴��� �����մϴ�
```
default: false
options: boolean (true / false)
```

**slideSelector**
�����̵�� ����� ��� (ex. <code>'div.slide'</code>).<br />����: �⺻������, bxSlider�� �����̴� ����� ��� ���� �ڽ��� ����մϴ�.
```
default: ''
options: jQuery selector
```

**infiniteLoop**
���� <code>true</code>�� �����ϸ�, �� ���������� "Next" �� Ŭ���ϸ� ó������ ��ȯ�˴ϴ�.
```
default: true
options: boolean (true / false)
```

**hideControlOnEnd**
`true`�� ��� �����̵尡 ù��° �Ǵ� �������϶� "Prev"�� "Next" ��Ʈ���� ��Ȱ��ȭ�ϴ� Ŭ����(`disabled`)�� �ްԵ˴ϴ�.<br/>����: <code>infiniteLoop: false</code> �� ����ϴ� ��츸 ����.
```
default: false
options: boolean (true / false)
```

**easing**
"easing" ������ ��ȯ�� ���. CSS ��ȯ�� ����ϴ� ���, <code>transition-timing-function</code> �Ӽ��� ���� ���� �����Ѵ�. CSS ��ȯ�� ������� �ʴ� ��� ����� ������ �ɼ� �÷������� <code>jquery.easing.1.3.js</code>�� ���� �� �� �ִ�.<br>�� ���� ������ ���Ͻø� [http://gsgd.co.uk/sandbox/jquery/easing/](http://gsgd.co.uk/sandbox/jquery/easing/)�� �����Ͻʽÿ�.

```
default: null
options: CSS�� ����ϴ� ���: 'linear', 'ease', 'ease-in', 'ease-out', 'ease-in-out', 'cubic-bezier(n,n,n,n)'. CSS�� ������� �ʴ� ���: 'swing', 'linear' (�߰� �ɼ��� ������ ���� ������ �����Ͻʽÿ�)
```

**captions**
�̹��� ĸ���� �����մϴ�. ĸ���� �̹����� <code>title</code> �Ӽ��Դϴ�.
```
default: false
options: boolean (true / false)
```

**ticker**
ticker ��忡�� �����̴��� ��� (���� ticker�� ����)
```
default: false
options: boolean (true / false)
```

**tickerHover**
���콺�� �����̴��� ����ų �� ticker�� �Ͻ� �����˴ϴ�. ���� :�� ����� CSS�� transitions�� ����ϴ� ��� �۵����� �ʽ��ϴ�!
```
default: false
options: boolean (true / false)
```

**adaptiveHeight**
�������� �� �����̵��� ���̸� ������� �����̴� ���̸� �����մϴ�.
```
default: false
options: boolean (true / false)
```

**adaptiveHeightSpeed**
�����̵� ���� ��ȯ �ð�(ms ����). ����: <code>adaptiveHeight: true</code>���� ���
```
default: 500
options: integer
```

**video**
��� �����̵� ������ �����ϴ� ���, <code>true</code>�� �����մϴ�. ����, �÷����� <code>jquery.fitvids.js</code>����<br />
�� ���� ������ ���Ͻø� [http://fitvidsjs.com/](http://fitvidsjs.com/) ����
```
default: false
options: boolean (true / false)
```

**responsive**
Ȱ�� �Ǵ� ��Ȱ������ �����̴��� ũ�������� �ڵ����� �����մϴ�..
```
default: true
options: boolean (true /false)
```

**useCSS**
`true`�� ���, CSS ��ȯ�� ���� �� ���� �����̵� �ִϸ��̼ǿ� ���� (����Ƽ�� �ϵ���� ������ ����մϴ�). `false`�� ���, jQuery�� animate()�� ���˴ϴ�.
```
default: true
options: boolean (true / false)
```

**preloadImages**
'all' �̸�, �����̴��� �����ϱ� ���� ��� �̹����� �̸��ε�. 'visible' �̸�, �����̴��� �����ϱ� ���� ó�� �� �����̵��� �̹����� �̸��ε� (tip: ��� �����̴��� ũ�Ⱑ �����Ѱ�� 'visible' ���)
```
default: 'visible'
options: 'all', 'visible'
```

**touchEnabled**
<code>true</code>�̸�, �����̴��� ��ġ swipe ��ȯ�� ����մϴ�
```
default: true
options: boolean (true / false)
```

**swipeThreshold**
�ȼ��� ���� ��ġ swipe �����̵� ��ȯ�� �����ϱ� ���� �ʰ� �� �ʿ䰡�ִ�. ����: <code>touchEnabled: true</code>���� ���
```
default: 50
options: integer
```

**oneToOneTouch**
If <code>true</code>, non-fade slides follow the finger as it swipes
```
default: true
options: boolean (true / false)
```

**preventDefaultSwipeX**
If <code>true</code>, touch screen will not move along the x-axis as the finger swipes
```
default: true
options: boolean (true / false)
```

**preventDefaultSwipeY**
If <code>true</code>, touch screen will not move along the y-axis as the finger swipes
```
default: false
options: boolean (true / false)
```

**wrapperClass**
Class to wrap the slider in. Change to prevent from using default bxSlider styles.
```
default: 'bx-wrapper'
options: string
```


###Pager

**pager**
<code>true</code>�̸�, pager�� �߰��˴ϴ�
```
default: true
options: boolean (true / false)
```

**pagerType**
<code>'full'</code>�̸�, pager ��ũ�� �� �����̵忡 ���� �����˴ϴ�. <code>'short'</code>�̸�, x / y pager�� ���˴ϴ� (ex. 1 / 5)
```
default: 'full'
options: 'full', 'short'
```

**pagerShortSeparator**
<code>pagerType: 'short'</code>�̸�, pager�� �и� ���ڷ� �� ���� ����մϴ�
```
default: ' / '
options: string
```

**pagerSelector**
pager �����ͷ� ������Ʈ�� ����մϴ�. �⺻������ ȣ���� bx-viewport�� �߰��˴ϴ�
```
default: ''
options: jQuery selector
```

**pagerCustom**
�θ� ��Ұ� pager�μ� �̿�ȴ�. �θ� ��Ҵ� �� �����̵忡 ���� <code>&lt;a data-slide-index="x"&gt;</code>�� �����ؾ��մϴ�. ������ ���� carousels�� �Բ� ����ؾ��մϴ�.
```
default: null
options: jQuery selector
```

**buildPager**
�����Ǵ� ���, �Լ��� ��� �����̵� ����̸�, ��ȯ�� ���� ������ �׸� ��ũ������ ���˴ϴ�. <br />�ڼ��� ���������� <a href="http://bxslider.com/examples">����</a>�� �����Ͻʽÿ�.
```
default: null
options: function(slideIndex)
```



###Controls

**controls**
<code>true</code>�̸�, "Next" / "Prev" ��Ʈ���� �߰��˴ϴ�
```
default: true
options: boolean (true / false)
```

**nextText**
�ؽ�Ʈ�� "Next" ��� ���˴ϴ�.
```
default: 'Next'
options: string
```

**prevText**
�ؽ�Ʈ�� "Prev" ��� ���˴ϴ�.
```
default: 'Prev'
options: string
```

**nextSelector**
"Next" ��� ����� ������Ʈ ���
```
default: null
options: jQuery selector
```

**prevSelector**
"Prev" ��� ����� ������Ʈ ���
```
default: null
options: jQuery selector
```

**autoControls**
<code>true</code>�̸�, "Start" / "Stop" ��Ʈ�� �߰�
```
default: false
options: boolean (true / false)
```

**startText**
�ؽ�Ʈ�� "Start" ��� ���˴ϴ�.
```
default: 'Start'
options: string
```

**stopText**
�ؽ�Ʈ�� "Stop" ��� ���˴ϴ�.
```
default: 'Stop'
options: string
```

**autoControlsCombine**
�����̵� � ����ϸ� "Stop" ��Ʈ���� ǥ�õǰ� �ݴ��� ��쵵 �������� �Դϴ�.
```
default: false
options: boolean (true / false)
```

**autoControlsSelector**
auto(�ڵ�����) ��� ���Ǵ� ������Ʈ ��Ҹ� �����մϴ�.
```
default: null
options: jQuery selector
```

**keyboardEnabled**
�����̴��� ���� Ű���� �׺���̼��� Ȱ��ȭ�մϴ�.
```
default: false
options: boolean (true / false)
```


###Auto

**auto**
�����̵尡 �ڵ��������� ��ȯ�˴ϴ�
```
default: false
options: boolean (true / false)
```
**stopAutoOnClick**
�ڵ������� �ߴܵ˴ϴ�
```
default: false
options: boolean (true / false)
```

**pause**
�ڵ����� ��ȯ ������ �ð�(ms ����)
```
default: 4000
options: integer
```

**autoStart**
�ε�ɶ� �ڵ������� �����մϴ�. ���� <code>false</code>�̸�, "Start" ��Ʈ���� Ŭ���ؾ� ���۵˴ϴ�.
```
default: true
options: boolean (true / false)
```

**autoDirection**
�ڵ����� ����Ǵ� �����̵� ��ȯ �����Դϴ�.
```
default: 'next'
options: 'next', 'prev'
```

**autoHover**
���콺�� �����̴��� ����ų �� �����̵尡 �Ͻ����� �˴ϴ�
```
default: false
options: boolean (true / false)
```

**autoDelay**
�ڵ������� ���۵Ǳ����� ��ٸ��� �ð��Դϴ�.
```
default: 0
options: integer
```



###Carousel

**minSlides**
�����̵��� �ּ� ���� ǥ���մϴ�. ĳ������ ���� ũ�⺸�� �۾��� ��� �����̵� ũ�Ⱑ �� ���Դϴ�.
```
default: 1
options: integer
```

**maxSlides**
�����̵��� �ִ� ���� ǥ���մϴ�. �����̾ ���� ũ�⺸�� Ŀ���� �����̵嵵 �ڵ� Ű�����ϴ�.
```
default: 1
options: integer
```

**moveSlides**
�̼����� �����̵�� �̵��մϴ�. �̰����� �ؾߵ˴ϴ� <code>>= minSlides</code>, �׸��� <code><= maxSlides</code>. ���� 0�ΰ�� (�⺻��), �����̵忡 ������ ���ڷ� �̵��˴ϴ�.
```
default: 0
options: integer
```

**slideWidth**
�� �����̵��� ���Դϴ�. �� ������ ��� ���� ĳ������ �ʿ��մϴ�!
```
default: 0
options: integer
```

**shrinkItems**
ĳ������ ��ü �׸��� ǥ���ϰ� maxSlides / MinSlides�� ������ ����Ʈ�� �°� �̹����� ����� ���̴�.
```
default: false
options: boolean (true / false)
```




###Keyboard

**keyboardEnabled**
�����̵带 Ű����� ���� �� �� �ֽ��ϴ�. �����̴��� �� �� ���� ��� Ű������(Keypress)�� �����մϴ�.
```
default: false
options: boolean (true / false)
```





### Accessibility

**ariaLive**
�����̵� �Ӽ��� Aria Live�� �߰��մϴ�.
```
default: true
options: boolean (true / false)
```

**ariaHidden**
������ �ʴ� �����̵忡 Aria Hidden �Ӽ��� �߰��մϴ�.
```
default: true
options: boolean (true / false)
```





###Callbacks

**onSliderLoad**
�����̴��� ������ �ε�� ���� ����
```
default: function(){}
options: function(currentIndex){ // your code here }
arguments:
  currentIndex: ���� �����̴��� �ε���
```

**onSliderResize**
�����̴��� ũ�Ⱑ ����� �� ��� ����
```
default: function(){}
options: function(currentIndex){ // your code here }
arguments:
  currentIndex: ���� �����̴��� �ε���
```

**onSlideBefore**
�����̵� ��ȯ ������ �����մϴ�.
```
default: function(){}
options: function($slideElement, oldIndex, newIndex){ // your code here }
arguments:
    $slideElement: �����(jQuery element)
    oldIndex: ���� �����̴��� �ε���(��ȯ��)
    newIndex: ���� �����̴��� �ε���(��ȯ��)
```

**onSlideAfter**
�����̵� ��ȯ �� ��� �����մϴ�. �Լ��� �μ��� ���� �����̵� ���(��ȯ�� �Ϸ� �� ��)�Դϴ�.
```
default: function(){}
options: function($slideElement, oldIndex, newIndex){ // your code here }
arguments:
    $slideElement: �����(jQuery element)
    oldIndex: ���� �����̴��� �ε���(��ȯ��)
    newIndex: ���� �����̴��� �ε���(��ȯ��)
```

**onSlideNext**
"Next" �����̵� ��ȯ ������ �����մϴ�. �Լ��� �μ��� ����� �����̵� (next)������Ʈ�Դϴ�.
```
default: function(){}
options: function($slideElement, oldIndex, newIndex){ // your code here }
arguments:
    $slideElement: �����(jQuery element)
    oldIndex: ���� �����̴��� �ε���(��ȯ��)
    newIndex: ���� �����̴��� �ε���(��ȯ��)
```

**onSlidePrev**
"Prev" �����̵� ��ȯ ������ �����մϴ�. �Լ��� �μ��� ����� �����̵� (prev)������Ʈ�Դϴ�.
```
default: function(){}
options: function($slideElement, oldIndex, newIndex){ // your code here }
arguments:
    $slideElement: �����(jQuery element)
    oldIndex: ���� �����̴��� �ε���(��ȯ��)
    newIndex: ���� �����̴��� �ε���(��ȯ��)
```




###Public methods

**goToSlide**
������ �����̵� �ε����� �����̵� ��ȯ�� �����մϴ� (zero-based)
```
example:
slider = $('.bxslider').bxSlider();
slider.goToSlide(3);
```

**goToNextSlide**
"Next" �����̵� ��ȯ�� �����մϴ�
```
example:
slider = $('.bxslider').bxSlider();
slider.goToNextSlide();
```

**goToPrevSlide**
"Prev" �����̵� ��ȯ�� �����մϴ�
```
example:
slider = $('.bxslider').bxSlider();
slider.goToPrevSlide();
```

**startAuto**
�����̵��� �ڵ�����(auto)�� �����մϴ�. ���� <code>false</code>�̸� ������Ʈ�Ǵ� �ڵ� ��Ʈ���� �����ϴ�.
```
example:
slider = $('.bxslider').bxSlider();
slider.startAuto();
```

**stopAuto**
�����̵��� �ڵ�����(auto)�� �����մϴ�. ���� <code>false</code>�̸� ������Ʈ�Ǵ� �ڵ� ��Ʈ���� �����ϴ�.
```
example:
slider = $('.bxslider').bxSlider();
slider.stopAuto();
```

**getCurrentSlide**
���� Ȱ��ȭ�� �����̵带 ��ȯ�մϴ�.
```
example:
slider = $('.bxslider').bxSlider();
var current = slider.getCurrentSlide();
```

**getSlideCount**
�����̵��� �� ������ ��ȯ�մϴ�.
```
example:
slider = $('.bxslider').bxSlider();
var slideQty = slider.getSlideCount();
```

**redrawSlider**
�����̵带 �ٽ� �׸��ϴ�. �����̵带 ������ �ٽ� ǥ���Ҷ� �����մϴ�.
```
example:
slider = $('.bxslider').bxSlider();
slider.redrawSlider();
```

**reloadSlider**
�����̵带 ���ε��մϴ�. �ǽð����� �����̵带 �߰��Ҷ� �����մϴ�. ������ �ɼ� ��ü�� �޾Ƶ��Դϴ�.
```
example:
slider = $('.bxslider').bxSlider();
slider.reloadSlider();
```

**destroySlider**
�����̴��� �ı�(destroy)�մϴ�. �̰��� (�����̴��� ȣ���ϱ� ����) �ٽ� ���� ���·� ��� �����̴� ��Ҹ� �ǵ����ϴ�.
```
example:
slider = $('.bxslider').bxSlider();
slider.destroySlider();
```


----


* [Jquery README](../README.md)
* [01_00_jquery_���ʹ���](01_00_jquery_���ʹ���.md)
* [01_00_jquery_���ֻ���ϴ�_�Լ�](01_00_jquery_���ֻ���ϴ�_�Լ�.md)
* [01_01_jquery_plugin_bxslider](01_01_jquery_plugin_bxslider.md)
* [01_02_jquery_plugin_slidesjs](01_02_jquery_plugin_slidesjs.md)
* [01_03_jquery_plugin_bpopup](01_03_jquery_plugin_bpopup.md)
* [jquery](jquery.md)
* [Datepicker](Datepicker.md)

----


* [FrontEndStudy](../../README.md)
