# jQuery ���ʹ���

## jQuery ����

### jQuery ������

�����ڸ� | ����
--- | ---
$('tag') | Tag��� �̸��� ��� �±� ��Ҹ� ����
$(��.class��) | class��� Ŭ�������� ��� Ŭ���� ��Ҹ� ����
$(��#id��) | id��� ���̵���� ���̵� ��Ҹ� ����
$(��div li��) | div�� �ִ� li ��� ����
$(��div > p��) | div�� p�±׶�� ���� �ڽ��� ����
$(this) | ���� ���� ���� ��Ҹ� ����Ŵ

### jQuery �޼ҵ�

�޼ҵ�� | ����
--- | ---
eq(n) | n��°�� ��ġ�ϴ� ��Ҹ� ����.
length() | ����� ������ �� �� ����.
parent()  /  parents() | ����� ���� �θ� ����  /  ����� ��� �θ�� ����
children(��a��) | ����� a�±��� �����ڼ� ����
prev()  /  next() | ���� ��� ����  /  ���� ��� ����
val() | �ؽ�Ʈ�� �Է��� ���� ����
text() | �ش� ����� �ؽ�Ʈ�� ����
move()  /  clone() | �ش� ��� �̵�  /  �ش� ��� ����
remove() | �ش� ��� ����
bind(�̺�Ʈ,�Լ�)  /  unbind(�̺�Ʈ) | �ش� �̺�Ʈ ����� �Լ� ���� / �̺�Ʈ ����
&nbsp; | * unbind() - �ش繮�� ��ü�� ���õ� ��� �̺�Ʈ ����
&nbsp; | * unbind(eventName) - Ư�� �̺�Ʈ�� ���õ� ��� �̺�Ʈ ����
&nbsp; | * unbind(eventName, function) - Ư�� �̺�Ʈ�� �Լ� ����
addClass()  /  removeClass() | Ŭ���� �߰�  /  Ŭ���� ����

### jQuery �̺�Ʈ
�̺�Ʈ�� | ����
--- | ---
mousedown() | ��念������ ���콺�� �����ٰ� ������ �� �߻�
mouseenter() | ��忡 ���콺�� �������� �� �߻� -> �θ� �������� �ڽĿ����� Ŀ���� ���� ���콺 �������� �Ǵ�
mouseleave() | ��念������ ���콺�� ������ �� �߻�
mousemove() | ��念������ ���콺�� ������ �� �߻�
mouseover() | ��� ������ ���콺�� �÷� ������ �� �߻� -> �θ� �������� �ڽĿ����� Ŀ���� ���� ���콺 �ƿ����� �Ǵ�
mouseup() | ���콺 �����͸� ��忡 �÷����� ���콺 ��ư�� ������ �� �߻�

### jQuery Ű���� �̺�Ʈ
Ű���� �̺�Ʈ�� | ����
--- | ---
keydown() | Ű���尡 ������ �� �߻�
keyup() | Ű���尡 ������ �� �߻�
keypress() | ���ڰ� �Էµ� �� �߻�

#### html()
* ���� ������ ���ְ� �ʿ��� html������ ������

```javascript
$subMenu1.html("<li>text</li>");
```

#### ������ ��ü ���� �� ����
* $(A).insertBefore(B) : A�� B�տ� �߰�
* $(C).insertAfter(B) : C�� B�ڿ� �߰�

* $(D).prependTo(B) : D�� B �պκп� �߰�
* $(E).appendTo(B) : E�� B�� �޺κп� �߰�

* $(1).after(F) : 1���� F ����
* $(3).before(G) : 3���� G ����

#### css()
* �ش� ����� CSS�� ���� �� �� ����

```javascript
// ex)
$("#header").css({height:80, overflow:"hidden"}) //height, overflow ����

// ex)
var $alpha=$(".subMenu").css("opacity"); //opacity �� ����
```


#### attr()
* �ش� ����� �Ӽ��� ���� �� �� ����

```javascript
// ex)
$mainImg.attr("class","img02");  //Ŭ������ ����

// ex)
$("#visual_img").attr("src", "images/main/visual_02.jpg") //�̹��� ��� ����

// ex)
var $className=$("#visual_img").attr("class"); //Ŭ������ �� ����
```

#### setInterval(�Լ���,�ֱ�)
* �����ð� ���� �Լ��� ����ǵ��� ó��

#### clearInterval(�Լ���)
* setInterval�� ������ �۾��� ���


## Animation

### Animate({�Ӽ�:��},�ð�,ȿ��,�Լ�)
* �Ӽ��� ����ŭ �ð��ֱ�� �ش�ȿ���� �� �� �Լ��� ������
* ȿ�� : jQuery�� easingȿ��(32������ easing ȿ�� ��� ����)

```javascript
//ex)
function onLeft() {
   #imgWrap.animate({marginLeft:-400},500,"easeOutCubic");
}
```

```javascript
//ex)
$("#imgWrap:not(:animated)").animate({left:300, opacity:0}, 1000, "easeOutCubic", function() {
   #imgWrap.css({left:0, opacity:1});
});
```


## Ȱ�밡���� jQuery ����

### Slide Image
* slideUP(), slideDown() ��� (left, right�� ���� �ȵ�)
* appendTo(), prependTo(), animate() ���

### Show, hide Image
* show(), hide() ���
* tab menu, modalWindow Ȱ�밡��

### Scroll Image
* scrollTop() ���


## Ư�̻���

### �۵� ���� ���� ����
* ���� �Լ����� �� �Լ��� ������ �������� �� ���ÿ� �ٸ� �Լ� ������ ���� ���ϵ��� ��.

```javascript
<script type="text/javascript">
var count;
var $panel;
var totalMember;
var timer;
var isPlay = false; //�۵� ���� ����, �������ڸ��ڴ� �۵����� ������ false

$(document).ready(function() {
   $panel = $("#panel");
   $(".btn_start").bind("click", onStart);
   $(".btn_stop").bind("click", onStop);
});

function onStart() {
   if(isPlay == false) {
      totalMember = parseInt($("#tatalWrap").val());
      timer = setInterval(onCount,20);
      isPlay = true;
   }
}

function onCount() {
   count = parseInt(Math.random()*totalMember)+1
   $panel.html(count);
   $panel.css("font-size", parseInt(Math.random()*100)+100)
   $panel.css("color", "black");
}
function onStop() {
   if(isPlay == true) {
      clearInterval(timer);
      $panel.css("color", "red");
      $panel.css("font-size", 200);
      isPlay = false;
   }
}
</script>
```

### :not(:animated)
* �ش� �ִϸ��̼��� �������� �� �ٸ� �ִϸ��̼� ������ ���ϵ��� ��.
* �ش� �ִϸ��̼��� �� ������ ���� �ִϸ��̼��� ���� ��.

```javascript
<script type="text/javascript">
var $mainMenu;
var $subMenu;
var $subBg;

$(document).ready(function(e) {
   $mainMenu = $(".menu_list > li");
   $subMenu = $(".subMenu");
   $subBg = $("#sub_bg");

   $subMenu.hide();
   $subBg.hide();

   $mainMenu.bind("mouseover", onOver);
   $subBg.bind("mouseout", onOut);

   function onOver() {
      //bg�� �������� ���� �ٸ� �̺�Ʈ�� �����Ű�� �ʴ´�.
      $("#sug_bg:not(:animated").slideDown(100, "easeOutCubic", function() {
         $subMenu.show();
      });
   }

   function onOut() {
      $subMenu.hide();
      $("#sub_bg:not(:animated)") .slideUp(300, "easeOutCubic");
   }
})
</script>
```

### stop()
* �������� �ִϸ��̼��� ��� ����.
* ���� �ִϸ��̼��� ���� ����� �����ϴ� �ִϸ��̼��� ���� �Ϸ� �� �ٸ� �ִϸ��̼� ����� ���.

```javascript
<script type="text/javascript">
var $menu;
$(document).ready(function(e) {
   $menu = $(".menu > li");
   $menu.bind("mouseenter", onOver);
   $menu.bind("mouseleave", onOut);
});

function onOver() {
   $(this).children("div").stop();
   $(this).children("div").animate({top:-30}, 300, "easeOutCubic");
}

function onOut() {
   $(this).children("div").stop();
   $(this).children("div").animate({top:0}, 300, "easeOutCubic");
}
</script>
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
