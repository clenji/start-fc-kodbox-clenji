
##### 1.30 更新内容
- 新建文件夹: 当前目录下已存在同名文件夹,并且在回收站中时处理;
- 上传或新建文件: 当前目录下已存在同名文件,并且在回收站中时处理;
##### 1.23 更新内容 (2021.4.1)
- office编辑保存逻辑处理兼容(保留历史版本,)
	- 上传~tmp1601041332501525796.TMP //锁定,上传,解锁;
	- 移动 test.docx => test~388C66.tmp 				// 改造,识别到之后不进行移动重命名;
	- 移动 ~tmp1601041332501525796.TMP => test.docx; 	// 改造;目标文件已存在则更新文件;删除原文件;
	- 删除 test~388C66.tmp  
- 无保存权限处理;

##### 1.22 更新内容 (2021.3.26)
- 粘贴文件为0字节问题兼容;
- 登陆日志记录; 
- 复制移动兼容处理; 支持移动到收藏的各类IO路径