# Perfect-DateTimePicker
---

> A jQuery plugin for Date and Time Picker(����jQuery������ʱ��ѡ����)

**Demo:** ![lalal](http://www.shaowenwu.cn)

###Example(����ʾ��)

```javascript
    var picker = $('#demo1').datetimepicker({
        date: new Date(),
        viewMode: 'YMDHMS',
        onDateUpdate: function(){
            $('#date-text').text(this.getText());
        },
        onClose: function(){
            this.element.remove();
        }
    });
```

###API(�ӿ�)

<table>
<th>
<tr><td>����</td><td>����</td><td>����</td></tr>
</th>
<tbody>
<tr><td>baseCls</td><td>String</td><td>����ʽ</td></tr>
<tr><td>viewMode</td><td>String</td><td>'YM'|'YMD'|'YMDHMS'|'HMS'</td></tr>
<tr><td>startDate</td><td>Date</td><td>��ʼ����</td></tr>
<tr><td>endDate</td><td>Date</td><td>��������</td></tr>
<tr><td>date</td><td>Date</td><td>��ǰֵ</td></tr>
<tr><td>onDateUpdate</td><td>Function</td><td>���ڸ����¼�</td></tr>
<tr><td>onClear</td><td>Function</td><td>�����ť�¼�</td></tr>
<tr><td>onOk</td><td>Function</td><td>ȷ�ϰ�ť�¼�</td></tr>
<tr><td>onClose</td><td>Function</td><td>�رհ�ť�¼�</td></tr>
<tr><td>onToday</td><td>Function</td><td>ѡȡ���찴ť�¼�</td></tr>
</tbody>
</table>
