# jQuery  ���� ����ϴ� �Լ�


## Triggrt �Լ�

���� ��ũ:  http://api.jquery.com/trigger/

```javascript
.trigger( eventType [, extraParameters] )
```

���� : Ư�� �̺�Ʈ ������ ���� ���õ� ��ҿ� ����� ��� �ڵ鷯�� ����(behavior)�� �����մϴ�.

```javascript
.trigger( eventType [, extraParameters] )
```

eventType: JavaScript �̺�Ʈ Ÿ���� ǥ���ϴ� ���ڿ�, `click` �Ǵ� `submit` ����.

extraParameters: �̺�Ʈ �ڵ鷯�� ������ �߰� �Ķ����.

.trigger( event )
event jQuery.Event ��ü.



<br>


## ����_01
.trigger() �Լ��� �̺�Ʈ�� �߻��� �� ����� �Լ��� .bind() �Լ��� ����� � �̺�Ʈ �ڵ鷯�� ������ ������� �ݴϴ�.

```javascript
$('#foo').bind('click', function() {
    alert($(this).text());
});
$('#foo').trigger('click');
```

`#foot` �����ڸ� Ŭ�� ���� �ʾƵ� trigger�Լ��� ����� click �̺�Ʈ��  trigger�Լ��� Ư¡�� ���Ͽ�
 `alert($(this).text());` ��  ������ �����մϴ�.


<br>

## ����_02

```html
<script>  
$(document).ready(function () {
    //btnŬ�� �̺�Ʈ ó��
    $("#btn").click(function () { alert('��ư�� Ŭ���Ǿ����ϴ�.') });
    //������ �ε�� ��ư Ŭ��
    $('#my .hover').click(function () { alert('��ư�� Ŭ��'); });
    $('#my input[type=button]').one("click", function () {
     alert('���� ��ư�� ����ڿ� ���ؼ� Ŭ����');
    });
    $('#btn').bind("click", function () { alert('��ư�� Ŭ����'); });
    //��ư Ŭ���� �ƴ϶� �ڵ忡 ���ؼ� click�̺�Ʈ�� �����ϰ� �ʹٸ�?
    $('#btn').trigger('click');
});
</script>

<!-- ��� click  �̺�Ʈ��   $('#btn').trigger('click'); �ڵ��� ���Ͽ�  ������ ����Ǵ� ���� �Դϴ�. -->

<div id="my">
   <input type="button" id="btn" value="��ư" class="hover" />
</div>
```






<br>

## each(�ݺ���) �Լ�

.each()�� ������ ��Ұ� �������� �� ������ ���Ͽ� �ݺ��Ͽ� �Լ��� �����ŵ�ϴ�.

����  :  .each( function )

Ư�� ������ ������ �� �ݺ� �۾����� ��������  :  return false ����մϴ�.



## ����_01

```html
<style>
  .s1 {color: red;}
  .s2 {color: blue;}
  .s3 {color: green;}
  .s4 {color: brown;}
</style>

<script>
  $( document ).ready( function() {
    var i=1
    $( 'p' ).each( function() {
      $( this ).addClass( 's' + i );
      i = i + 1;
    } );
  } );
</script>


<p>Lorem</p>
<p>Ipsum</p>
<p>Dolor</p>
<p>Amet</p>
```



## ����_02
�ݺ� �۾��� �ι��� �ϰ� ���������� �����Դϴ�.

```html
<style>
  .s1 {color: red;}
  .s2 {color: blue;}
  .s3 {color: green;}
  .s4 {color: brown;}
</style>

<script>
  $( document ).ready( function() {
    var i=1
    $( 'p' ).each( function() {
      $( this ).addClass( 's' + i );
      i = i + 1;
      if ( i == 3 ) {
        return false;
      }
    } );
  } );
</script>

<p>Lorem</p>
<p>Ipsum</p>
<p>Dolor</p>
<p>Amet</p>
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
