# Perfect-DateTimePicker
---

## A jQuery plugin for Date and Time Picker(����jQuery������ʱ��ѡ����)

**Demo:** [http://finexs.github.io/Perfect-DateTimePicker](http://finexs.github.io/Perfect-DateTimePicker)

###Preview(Ԥ��ͼ)
![](https://github.com/FineXs/Perfect-DateTimePicker/blob/master/examples/1.png)
![](https://github.com/FineXs/Perfect-DateTimePicker/blob/master/examples/2.png)
![](https://github.com/FineXs/Perfect-DateTimePicker/blob/master/examples/3.png)

###API(�ӿ�)

* ��������

<table>
<tr><td><b>����</b></td><td><b>����</b></td><td><b>����</b></td></tr>
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
</table>

* ���ýӿ�

<table>
<tr><td><b>����</b></td><td><b>����</b></td><td><b>����</b></td><td><b>����</b></td></tr>
<tr><td>getValue</td><td>Function</td><td>��</td><td>��ȡ��ǰ���ڶ���</td></tr>
<tr><td>getText</td><td>Function</td><td>format(��ѡ�����ڸ�ʽ������: 'yyyy-MM-dd HH:mm:ss')</td><td>��ȡ��ǰ���ڵ��ı���ʽ</td></tr>
<tr><td>element</td><td>Object</td><td>��</td><td>����ѡ������jQuery����</td></tr>
<tr><td>$datetable</td><td>Object</td><td>��</td><td>��������ѡ������jQuery����</td></tr>
<tr><td>$monthtable</td><td>Object</td><td>��</td><td>��������ѡ������jQuery����</td></tr>
<tr><td>$timetable</td><td>Object</td><td>��</td><td>����ʱ��ѡ������jQuery����</td></tr>
</table>

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
    console.log(picker.getText());
    console.log(picker.getValue());
    picker.element.hide();
```

###Compatible(�����������)
IE8+

###License(Э��)
[MIT license](https://github.com/FineXs/Perfect-DateTimePicker/blob/master/LICENSE)

