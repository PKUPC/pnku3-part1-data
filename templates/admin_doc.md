这里是写给 admin 看的一些备忘录，主要记录一些没有 GUI 的神秘设置选项。

封禁功能：在 admin 页面的 Team 中，直接编辑 Team 的 Extra Info 信息，格式如下：


```json
{
	"ban_list": {
		"ban_message_until": "2024-07-19 05:48",
		"ban_manual_hint_until": "2024-07-19 05:48",
		"ban_recruiting_until": "2024-07-19 05:48"
	}
}
```

不是每一条都要填的，如果只要 ban 站内信，直接像下面这样填也行。
```json
{
	"ban_list": {
		"ban_message_until": "2024-07-19 05:48"
	}
}
```

注意！！日期必须符合这个规则，年（杠）月（杠）日（空格）小时（冒号）分钟，年必须 4 位，月必须 2 位， 日必须 2 位，小时必须 2 位，分钟必须 2 位，不足的补前导 0。
