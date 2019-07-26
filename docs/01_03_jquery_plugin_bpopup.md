# bpopup

bPopup.js  : 
* [���۷��� ����Ʈ : http://dinbror.dk/bpopup/ ] (http://dinbror.dk/bpopup/)
* v0.11.0 �ٿ�ε� :  [jquery.bpopup.min.js ] (https://raw.github.com/dinbror/bpopup/master/jquery.bpopup.min.js)



### Ư¡
* ����/���� �ڵ� ���� �� �������� ���� (������ ���̿� ���� absolut | fixed �ڵ�����)   
* �����˾� ���� (�������� �˾��� �� �� ������, ���� ���� �������� ����)
* �ݹ� ����
* Ajax, image, iframe ����
* ���� ������ tested :  Internet Explorer 6*-9, Firefox 2+, Opera 9+, Safari 4+ and Chrome 4+



### �⺻����

```html
<!doctype html>
<html>
<head>
	<meta charset="uft-8">
	<script src="http://code.jquery.com/jquery-latest.min.js"></script>
	<script src="./jquery.bpopup.min.js"></script>
	<script type="text/javascript">
		/* auto */
		$(window).load(function(){
			$('#bpopupLayer').bPopup({
				//option
			});
		});
		/* click */
		$('#bpopupBtn').click(function(){
			$('#bpopupLayer').bPopup({
				//option
			});
		});
	</script>
</head>
<body>
	<a href="#" id="bpopupBtn">bpopup Open </a>
	<div id="bpopupLayer">
		<span class="bClose">close</span>
		<p>popup Layer</p>
	</div>
</body>
</html>
```

* [=> codepen ����] (http://codepen.io/dot2flower/pen/LpwajB/)



## ����

**option**
�⺻�ɼ�
``` javascript
$('element_to_pop_up').bPopup(
	follow: [false, false], 
	// true or false (boolean) | x, y 
	// default : true
	// �˾��� ����ٴϴ� ���� ������ų �� ������, ���ʸ� ���� ����

	position: [150, 400], 
	// int |  x, y 
	// default : auto 
	// �˾� ��ǥ

	modalClose: false,  
	// true or false 
	// default : true
	// ����� ������ �˾� �ݱ� ����

	autoClose: 1000 ,
	//Auto closes after 
	// �ڵ� �ݱ� (�и���)

	opacity: 0.6, 
	// default : 0.7 	
	//��� ����

	positionStyle: 'fixed', 
	//'fixed' or 'absolute'
	// default : auto
	// �˾��� position ����
	
	fadeSpeed: 'slow', 
	// ������� �ӵ� 'slow', 'fast' or int

	followSpeed: 1500, 
	//����ٴϴ� �ӵ� 'slow' or 'fast' or int

	modalColor: 'yellow' , 	
	// default : #000	
	// ����� �÷� 

	easing: 'easeOutBack', 
	//uses jQuery easing plugin 

	speed: 450, 
	//���ϸ��̼� �ӵ�

	transition: 'slideDown', 
	// 'slideDown' or  'slideIn'
	// �˾� ���� �� �ִϸ��̼� �ɼ� 
	
	transitionClose: 'slideBack' 
	// �˾� ���� �� �ִϸ��̼� �ɼ�

);
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
