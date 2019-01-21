# captcha
验证码，兼容py2,py3

将验证码保存到内存中，然后输出

	在py2中是从cStringIO模块导入StringIO 
	out = StringIO()
	image.save(out, format=fmt)


	在py3中没有cStringIO模块了
	是 from io import BytesIO
	写到BytesIO即
	out = BytesIO()
	image.save(out, format=fmt)
  

或用兼容模块，在py2,3中都可以使用

	from six import BytesIO
