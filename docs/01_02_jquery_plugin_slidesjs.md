# slidejs
http://slidesjs.com


<br>

### ����

```html
<!doctype html>
<head>
    <style>
        /* Prevents slides from flashing */
        #slides {
            display:none;
        }
    </style>

    <script src="http://code.jquery.com/jquery-latest.min.js"></script>
    <script src="jquery.slides.min.js"></script>

    <script>
        $(function(){
            $("#slides").slidesjs({
                width: 940,
                height: 528
            });
        });
    </script>
</head>
<body>
    <div id="slides">
        <img src="http://placehold.it/940x528">
        <img src="http://placehold.it/940x528">
        <img src="http://placehold.it/940x528">
        <img src="http://placehold.it/940x528">
        <img src="http://placehold.it/940x528">
    </div>
</body>
```


<br>

### �ɼ�

```javascript
$(function() {
    $("#slides").slidesjs({
        width: 800, // ����
        height: 500, // ����
        start: 3, // ���� �̹��� ��ȣ
        navigation: {
            active: false // �׺���̼� ��� ����(���� ���� ���� ��ư)
            effect: "slide"
            //<a href="#" class="slidesjs-previous slidesjs-navigation">����</a>
            //<a href="#" class="slidesjs-next slidesjs-navigation">����</a>
            //false �� �̷������� ������ Ŀ���͸���¡ ������
        },
        pagination: {
            active: true, //����¡
            effect: "slide" //���� �������� ȿ�� �����̵�(slide) ���̵�ȿ��(fade)
            //css slidesjs-pagination �̺κ� �������� Ŀ���͸���¡ ������
        },
        play: {
            active: true,  //�÷��� ��ž��ư �������(��ư����Ұ�)
            effect: "slide", //ȿ�� slide, fade
            interval: 2000,  //�и������� ���� 5000 �̸� 5��
            auto: true, //���۽� �ڵ� ��� �������
            swap: true, //�÷��̽� ��ž��ư �Ѵٺ��� false, �ϳ��� ���� true
            pauseOnHover: false, //���콺 �÷����� �����̵� �����Ҳ��� ������
            restartDelay: 2500 //���콺 �÷ȴٰ� ���� ������ �� �۵� �ð� �и������� ����
            //css slidesjs-play, slidesjs-stop �̺κ��� �̿��ؼ� Ŀ���͸���¡ ������
        },
        effect: {
            slide: {
                // �����̵� ȿ��
                speed: 200
                // 0.2�ʸ��� �ٲ�
            },
            fade: {
                // ���̵� ȿ��
                speed: 300,
                // 0.3�ʸ��� �ٲ�
                crossfade: true
                // �����̹����� ���ļ� ��Ÿ�� ����
            }
        },
        callback: {
            loaded: function(number) {
                //ó�� ȭ�� �ε�ɶ� ��ȣ
                //  alert('loaded : ' + number);
                $('#slidesjs-slide-number').text(number);
            },
            start: function(number) {
                //������ ������ȣ
                //  alert('start : ' + number);
            },
            complete: function(number) {
                //������ ������ȣ
                //  alert('complete : ' + number);
                $('#slidesjs-slide-number').text(number);
            }
        }
    })
})
```



###����

* [ǥ�� �����̵�] (http://slidesjs.com/examples/standard/)
* [��� �� �����ϴ� �����̵�](http://slidesjs.com/examples/playing/)
* [�������� �����̵�](http://slidesjs.com/examples/multiple/)
* [�ݹ��� ���](http://slidesjs.com/examples/callbacks/)
* [�⺻ �����̵� �����̵� (��Ÿ���� ������� ����)](http://slidesjs.com/examples/basic/)
* [�⺻ ���̵� �����̵� (��Ÿ���� ������� ����)](http://slidesjs.com/examples/basic-fade/)



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
