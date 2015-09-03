# Perfect-DateTimePicker
---

## A jQuery plugin for Date and Time Picker(����jQuery������ʱ��ѡ����)

**Demo:** ![lalal](http://www.shaowenwu.cn)

###Example(����ʾ��)

```javascript
    $('#demo1').datetimepicker({
        date: new Date(),
        viewMode: 'YMDHMS',
        onDateUpdate: function(){
            $('#date-text').text(this.getText());
            $('#date-text-ymd').text(this.getText('yyyy-MM-dd'));
            $('#date-value').text(this.getValue());
        }
    });
```

###API(�ӿ�)

|---|---|---|
|����|����|����|
|---|---|---|
|baseCls|String|����ʽ|
|viewMode|String|����ʽ|
|startDate|Date|��ʼ����|
|endDate|Date|��������|
|date|Date|��ǰֵ|
|onDateUpdate|Function|���ڸ����¼�|
|onClear|Function|�����ť�¼�|
|onOk|Function|ȷ�ϰ�ť�¼�|
|onClose|Function|�رհ�ť�¼�|
|onToday|Function|ѡȡ���찴ť�¼�|
