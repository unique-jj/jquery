# jQuery


<br>

<table>
	<tr>
		<th>�з�</th>
		<th>����</th>
		<th>������Ƽ �� �ż���</th>
	</tr>
	<tr>
		<td rowspan="4">�Ϲݳ��ã��</td>
		<td>���̵�� ã��</td>
		<td>$('#���̵�')</td>
	</tr>
	<tr>
		<td>���̵�� ã��</td>
		<td>$('#���̵�')</td>
	</tr>
	<tr>
		<td>Ŭ�����̸�����</td>
		<td>$('Ŭ�����̸�')</td>
	</tr>
	<tr>
		<td>�Ӽ����� ã��</td>
		<td>$('[�Ӽ��̸�=��]')</td>
	</tr>
	<tr>
		<td rowspan="7">ã����� <br>�ٷ��</td>
		<td>ã�� ���� ���ϱ�</td>
		<td>$���.length</td>
	</tr>
	<tr>
		<td>n��° ��� �����ϱ�</td>
		<td>$���.eq(index)</td>
	</tr>
	<tr>
		<td>DOM ��ü����</td>
		<td>$���.get(index) , $���[index]</td>
	</tr>
	<tr>
		<td>���������� �����ϱ�</td>
		<td>
			<p>$���.each(function(index) {</p>
			<p>&nbsp;&nbsp; $(this) �Ǵ� $���.eq(index)</p>
			<p>})</p>
<!-- <pre><code>
$���.each(function(index) {
	$(this) �Ǵ� $���.eq(index)
})
</code></pre> -->
		</td>
	</tr>
	<tr>
		<td>����߿��� Ư����常 ã��</td>
		<td>$���.filter('������')</td>
	</tr>
	<tr>
		<td>����� �ڼճ���� Ư����� ã��</td>
		<td>$���.find('������')</td>
	</tr>
	<tr>
		<td>�ε��� �� ���ϱ�</td>
		<td>
			<p>$���.index()</p>
			<p>$���.index($���)</p>
			<p>$���.index(���DOM��ü)</p>
		</td>
	</tr>

	<tr>
		<td rowspan="5">�ڽĳ��ã��</td>
		<td>��� �ڽ� ��� ã��</td>
		<td>$���.children()</td>
	</tr>
	<tr>
		<td>Ư���ڽĳ�常 ã��</td>
		<td>$���.children('������')</td>
	</tr>
	<tr>
		<td>ù��° �ڽ� ��� ã��</td>
		<td>
			<p>$���.children().first()</p>
			<p>$���.children().eq(0)</p>
			<p>$���.children(':first')</p>
			<p>$���.children(':eq(0)')</p>
		</td>
	</tr>
	<tr>
		<td>��������° �ڽ� ã��</td>
		<td>
			<p>$���.children().last()</p>
			<p>$���.children(':last')</p>
			<p>$���.children().eq($���.children().length-1)</p>
			<p>$���.children(':eq('+$���.children().length-1+')')</p>
			<p>$���.children().eq(-1)</p>
			<p>$���.children(':eq(-1)')</p>
		</td>
	</tr>
	<tr>
		<td>n��° �ڽĳ��ã��</td>
		<td>
			<p>$���.children().eq(index)</p>
			<p>$���.children(':eq('+index=')')</p>
		</td>
	</tr>
	<tr>
		<td rowspan="2">�θ� ���ã��</td>
		<td>�θ� ���ã��</td>
		<td>$���.parent()</td>
	</tr>
	<tr>
		<td>���� ���ã��</td>
		<td>$���.parents(['������'])</td>
	</tr>
	<tr>
		<td rowspan="2">���� ���ã��</td>
		<td>���� ���� ���ã��</td>
		<td>
			<p>$���.prev()</p>
			<p>$���.prevAll(['������'])</p>
		</td>
	</tr>
	<tr>
		<td>���� ���� ���ã��</td>
		<td>
			<p>$���.next()</p>
			<p>$���.nextAll(['������'])</p>
		</td>
	</tr>

	<tr>
		<td rowspan="5">��� ����/�߰�</td>
		<td>��� ����</td>
		<td>$('�߰����Dom ���ڿ�')</td>
	</tr>
	<tr>
		<td>ù��° �ڽĳ���߰�</td>
		<td>
			<p>$�θ���.prepend($�߰����)</p>
			<p>$�߰����.prependTo($�θ���)</p>
		</td>
	</tr>
	<tr>
		<td>��������° �ڽĳ���߰�</td>
		<td>
			<p>$�θ���.append($�߰����)</p>
			<p>$�߰����.appendTo($�θ���)</p>
		</td>
	</tr>
	<tr>
		<td>Ư������� ������ġ�� �߰�</td>
		<td>
			<p>$�߰����.insertBefore($���س��)</p>
			<p>$���س��.before($�߰����)</p>
		</td>
	</tr>
	<tr>
		<td>Ư������� ������ġ�� �߰�</td>
		<td>
			<p>$�߰����.insertAfter($���س��)</p>
			<p>$���س��.after($�߰����)</p>
		</td>
	</tr>

	<tr>
		<td rowspan="4">��� �̵�</td>
		<td>ù��° �ڽ� ���� �̵�</td>
		<td>
			<p>$�θ���.prepend($�̵����)</p>
			<p>$�̵����.prependTo($�߰����)</p>
		</td>
	</tr>
	<tr>
		<td>��������° �ڽ� ���� �̵�</td>
		<td>
			<p>$�θ���.append($�̵����)</p>
			<p>$�̵����.appendTo($�߰����)</p>
		</td>
	</tr>
	<tr>
		<td>Ư�� ����� ���� ���� �̵�</td>
		<td>
			<p>$�̵����.insertBefor($���س��)</p>
			<p>$���س��.before($�̵����)</p>
		</td>
	</tr>
	<tr>
		<td>Ư�� ����� ���� ���� �̵�</td>
		<td>
			<p>$�̵����.insertAfter($���س��)</p>
			<p>$���س��.after($�̵����)</p>
		</td>
	</tr>
	<tr>
		<td rowspan="2">��� ����</td>
		<td>Ư�� ��� ����</td>
		<td>$���.remove()</td>
	</tr>
	<tr>
		<td>��� �ڽ� ��� ����</td>
		<td>$���.children().remove()</td>
	</tr>

	<tr>
		<td rowspan="4">��� ���� <br>�б� �� ����</td>
		<td>��� ������ ���ڿ��� �б�</td>
		<td>
			<p>$���.html() // �±׳�������</p>
			<p>$���.text() // �±׳�������</p>
		</td>
	</tr>
	<tr>
		<td>��� ���� �����ϱ�</td>
		<td>
			<p>$���.html('������ �±� ���ڿ�')</p>
			<p>$���.text('������ �ؽ�Ʈ')</p>
		</td>
	</tr>
	<tr>
		<td>��峻���� �̿��� �������� �ڽ� ��� �߰��ϱ�</td>
		<td>$���.html('�߰��� �±� ���ڿ�')</td>
	</tr>
	<tr>
		<td>��� ������ �̿��� ��� �ڽ� ��� �����ϱ�</td>
		<td>$���.html(')</td>
	</tr>

	<tr>
		<td rowspan="4">��Ÿ�� �ٷ��</td>
		<td>��Ÿ�� �� ���ϱ�</td>
		<td>
			<p>$���.css('��Ÿ�ϼӼ��̸�')</p>
			<p>$���.css(['��Ÿ�ϼӼ��̸�',])</p>
		</td>
	</tr>
	<tr>
		<td>��Ÿ�� �� �����ϱ�</td>
		<td>
			<p>$���.css('��Ÿ�ϼӼ��̸�', ��)</p>
			<p>$���.css({'��Ÿ�ϼӼ��̸�': ��, '��Ÿ�ϼӼ��̸�': ��})</p>
		</td>
	</tr>
	<tr>
		<td>Ŭ���� �߰�</td>
		<td>
			<p>$���.addClass('Ŭ�����̸�')</p>
			<p>$���.addClass('Ŭ�����̸�1 Ŭ�����̸�2 ...')</p>
		</td>
	</tr>
	<tr>
		<td>Ŭ���� ����</td>
		<td>
			<p>$���.removeClass('Ŭ�����̸�')</p>
			<p>$���.removeClass('Ŭ�����̸�1 Ŭ�����̸�2 ...')</p>
		</td>
	</tr>
	<tr>
		<td rowspan="2">�Ӽ� �ٷ��</td>
		<td>�Ӽ��� ���ϱ�</td>
		<td>
			<p>$���.attr('�Ӽ��̸�')</p>
			<p>$���.data('data-�Ӽ��̸�')</p>
		</td>
	</tr>
	<tr>
		<td>�Ӽ��� �����ϱ�</td>
		<td>
			<p>$���.attr('�Ӽ��̸�', '��')</p>
			<p>$���.data('data-�Ӽ��̸�', '��')</p>
		</td>
	</tr>

	<tr>
		<td rowspan="7">�̺�Ʈ �ٷ��</td>
		<td>�Ϲ� �̺�Ʈ ���</td>
		<td>$���.on('�̺�Ʈ�̸�', �̺�Ʈ������)</td>
	</tr>
	<tr>
		<td>���� �̺�Ʈ ���</td>
		<td>$���.�����̺�Ʈ(�̺�Ʈ������)</td>
	</tr>
	<tr>
		<td>����� �̺�Ʈ ����</td>
		<td>
			<p>$���.off('click', �����ϰ� ���� �̺�Ʈ�����ʸ�)</p>
			<p>$���.off('click')</p>
			<p>$���.off()</p>
		</td>
	</tr>
	<tr>
		<td>�̺�Ʈ �ѹ��� ����</td>
		<td>$���.one(�̺�Ʈ�̸�, �̺�Ʈ������)</td>
	</tr>
	<tr>
		<td>�⺻ �ൿ ���</td>
		<td>�̺�Ʈ��ü.preventDefault()</td>
	</tr>
	<tr>
		<td>���� ���߱�</td>
		<td>�̺�Ʈ��ü.stopPropagation()</td>
	</tr>
	<tr>
		<td>����Ȱ�� �ϳ��� �̺�Ʈ</td>
		<td>$���.on('�̺�Ʈ��', '������', �̺�Ʈ������)</td>
	</tr>

	<tr>
		<td rowspan="5">����� ��ġ <br>�� <br>ũ�� ���ñ��</td>
		<td>�θ� ��ǥ ��� ���ϱ�</td>
		<td>$���.offsetParent()</td>
	</tr>
	<tr>
		<td>���� ��ǥ ��ġ �ٷ��</td>
		<td>
			<p>������ǥ ��ġ ���ϱ�</p>
			<p>$���.position().left</p>
			<p>$���.position().top</p>
			<p>&nbsp;</p>
			<p>������ǥ ��ġ �����ϱ�</p>
			<p>$���.css('left', ��ġ��)</p>
			<p>�Ǵ�</p>
			<p>$���.css({left: ��ġ��, top: ��ġ��})</p>
		</td>
	</tr>
	<tr>
		<td>���� ��ǥ ��ġ �ٷ��</td>
		<td>
			<p>������ǥ ��ġ ���ϱ�</p>
			<p>$���.offset().left</p>
			<p>$���.offset().top</p>
			<p>&nbsp;</p>
			<p>������ǥ ��ġ �����ϱ�</p>
			<p>$���.offset({left: ��ġ��, top: ��ġ��})</p>
		</td>
	</tr>
	<tr>
		<td>��� ũ�� �ٷ��</td>
		<td>
			<p>�⺻ ũ�� ���ϱ�</p>
			<p>$���.width()</p>
			<p>$���.height()</p>
			<p>&nbsp;</p>
			<p>�⺻ ũ�� + padding ũ�� ���ϱ�</p>
			<p>$���.innerWidth()</p>
			<p>$���.innewHeight()</p>
			<p>&nbsp;</p>
			<p>�⺻ũ�� + padding + border ũ�� ���ϱ�</p>
			<p>$���.outerWidth()</p>
			<p>$���.outerHeight()</p>
			<p>&nbsp;</p>
			<p>�⺻ũ�� + padding + border + margin ũ�� ���ϱ�</p>
			<p>$���.outerWidth(true)</p>
			<p>$���.outerHeight(true)</p>
			<p>&nbsp;</p>
			<p>�⺻ ũ�� �����ϱ�</p>
			<p>$���.width(ũ�Ⱚ)</p>
			<p>$���.height(ũ�Ⱚ)</p>
			<p>&nbsp;</p>
			<p>�⺻ ũ�� + padding ũ�� �����ϱ�</p>
			<p>$���.innerWidth(ũ�Ⱚ)</p>
			<p>$���.innerHeight(ũ�Ⱚ)</p>
		</td>
	</tr>
	<tr>
		<td>��� ��ũ�� ��ġ �ٷ��</td>
		<td>
			<p>��ũ�� ��ġ ���ϱ�</p>
			<p>$���.scrollLeft()</p>
			<p>$���.scrollTop()</p>
			<p>&nbsp;</p>
			<p>��ũ�� ��ġ �����ϱ�</p>
			<p>$���.scrollLeft(��ġ��)</p>
			<p>$���.scrollTop(��ġ��)</p>
		</td>
	</tr>

	<tr>
		<td>������ ��ġ <br>�� ũ�� ���� ���</td>
		<td>���� ũ�� ���ϱ�</td>
		<td>
			<p>$(document).width()</p>
			<p>$(document).height()</p>
		</td>
	</tr>
	<tr>
		<td rowspan="7">ȭ���� ��ġ <br>�� <br>ũ�� ���ñ�� <br><br>�������� ��ġ <br>�� <br>ũ�� ���ñ��</td>
		<td>��ü ȭ�� ũ�� ���ϱ�</td>
		<td>
			<p>screen.width</p>
			<p>screen.height</p>
		</td>
	</tr>
	<tr>
		<td>��ȿ�� ��ü ȭ�� ũ�� ���ϱ�</td>
		<td>
			<p>screen.availWidth</p>
			<p>screen.availHeight</p>
		</td>
	</tr>
	<tr>
		<td>������ ũ�� ���ϱ�</td>
		<td>
			<p>�⺻ ũ�� ���ϱ�</p>
			<p>window.innerWidth</p>
			<p>window.innerHeight</p>
			<p>&nbsp;</p>
			<p>�⺻ ũ��+�޴���+���� ������ ���Ե� ũ�� ���ϱ�</p>
			<p>$(window).width()</p>
			<p>$(window).height()</p>
			<p>&nbsp;</p>
			<p>�⺻ ũ��+�޴���+����+��ũ�ѹ� ������ ���Ե� ũ�� ���ϱ�</p>
			<p>window.outerWidth</p>
			<p>window.outerHeight</p>
		</td>
	</tr>
	<tr>
		<td>������ ũ�� �����ϱ�</td>
		<td>window.resizeTo(width, height)</td>
	</tr>
	<tr>
		<td>������ ���� �̺�Ʈ ó��</td>
		<td>$(window).on('resize', function(){})</td>
	</tr>
	<tr>
		<td>������ ��ġ �ٷ��</td>
		<td>
			<p>��ġ�� ���ϱ�</p>
			<p>window.screenLeft</p>
			<p>window.screenTop</p>
			<p>&nbsp;</p>
			<p>��ġ�� �����ϱ�</p>
			<p>window.moveTo(dx, dy)</p>
			<p>window.moveBy(dx, dy)</p>
		</td>
	</tr>
	<tr>
		<td>������ ��ũ�� �ٷ��</td>
		<td>
			<p>��ũ�� ��ġ�� ���ϱ�</p>
			<p>window.pageXOffset</p>
			<p>window.pageYOffset</p>
			<p>&nbsp;</p>
			<p>��ũ�� ��ġ �����ϱ�</p>
			<p>window.scrollTo(x, y)</p>
			<p>window.scrollBy(x, y)</p>
			<p>&nbsp;</p>
			<p>��ũ�� �̺�Ʈ ó���ϱ�</p>
			<p>$(window).on('scroll', function(){})</p>
		</td>
	</tr>
	<tr>
		<td rowspan="2">���콺�� ��ġ �� ũ�� ���ñ��</td>
		<td>Ŭ���� ���� ��ġ</td>
		<td>
			<p>������ ������ �������� �ϴ� ���� ��ġ</p>
			<p>mouseEvent.clientX</p>
			<p>mouseEvent.clientY</p>
			<p>&nbsp;</p>
			<p>���� ������ �������� �ϴ� ���� ��ġ</p>
			<p>mouseEvent.pageX</p>
			<p>mouseEvent.pageY</p>
		</td>
	</tr>
	<tr>
		<td>Ŭ���� ���� ��ġ</td>
		<td>
			<p>var offsetX = mouseEvent.pageX - $(ŸŶ).offset()</p>
			<p>var offsetY = mouseEvent.pageY - $(ŸŶ).offset()</p>
		</td>
	</tr>

	<tr>
		<td rowspan="3">�Ϲ� ȿ�� �ٷ��</td>
		<td>��Ÿ���� ������� ȿ��</td>
		<td>
			<p>��Ÿ����</p>
			<p>$���.show()</p>
			<p>&nbsp;</p>
			<p>�������</p>
			<p>$���.hide()</p>
		</td>
	</tr>
	<tr>
		<td>���̵� ��/�ƿ� ȿ��</td>
		<td>
			<p>���̵� ��</p>
			<p>$���.fadeIn()</p>
			<p>&nbsp;</p>
			<p>���̵� �ƿ�</p>
			<p>$���.fadeOut()</p>
		</td>
	</tr>
	<tr>
		<td>�����̵� ��/�ٿ� ȿ��</td>
		<td>
			<p>�����̵� ��</p>
			<p>$���.slideUp()</p>
			<p>&nbsp;</p>
			<p>�����̵� �ٿ�</p>
			<p>$���.slideDown()</p>
		</td>
	</tr>
</table>



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
