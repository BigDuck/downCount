DownCount
=========

jQuery countdown plugin that accounts for timezone.
#改动wupeiji587@foxmail.com
修改原有代码，增加了在指定秒数触发的指定事件
#Usage

```JS
$('.countdown').downCount({
    date: '08/27/2013 12:00:00',
    offset: -5,
    warning:[5,10],
    warningFun:[function(){console.log("还剩下5秒的提醒函数")},function(){console.log("还剩下10秒的提醒函数")}]
}, function () {
    alert('WOOT WOOT, done!，结束的提醒函数');
});
```

#Options
Option | Description
---|---
date | Target date, ex `08/27/2013 12:00:00`
offset | UTC Timezone offset

You can also append a callback function which is called when countdown finishes.
