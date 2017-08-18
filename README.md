## Bootstrap及其插件记录

- BootstrapValidator（html/bootstrapValidator）
	- typicalValidator.html: 常用的验证器
	
	```
	validators: {
	    notEmpty: {
		message: '姓名不能为空'
	    },
	    stringLength: {
		min: 2,
		max: 20,
		message: '姓名长度为2~20个字符'
	    },
	    between: {
		min: 0,
		max: 132,
		inclusive: true, // 默认为true；设置为true，则取值范围为[0,132]；设置为false，则取值范围为(0,132)
		message: '年龄必须在0~132岁之间'
	    },
	    regexp: {
		regexp: /^(((13[0-9]{1})|(15[0-9]{1})|(18[0-9]{1}|(17[0-9]{1})))+\d{8})$/,
		message: '手机号码格式不正确'
	    },
	    regexp: {
		regexp: /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/,
		message: '邮箱地址格式不正确'
	    },
	    different: {
		field: 'oldPassword',
		message: '新密码不能与当前密码相同'
	    },
	    identical: {
		field: 'newPassword',
		message: '两次输入的密码不一致'
	    }
	}
	```
	
