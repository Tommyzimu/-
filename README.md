	不管电脑上有没有python软件都能够运行项目，不需要在每一个工程中都创建一个虚拟环境（而是将环境创建在工程目录中）
		方法实现：
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~$ workon env1			
			在当前目录下创建项目文件夹
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~$ mkdir project  * 此时在虚拟环境env1下
			进入到项目文件夹
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~$ cd project/
			创建 manage.py文件
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ touch manage.py
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ ls
			manage.py
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ mkdir project
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ ls
			manage.py  project
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ touch requirement.txt
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ vim requirement.txt 
			deactivate 退出虚拟环境
			(env1) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ deactivate 
			virtualenv env2 在项目文件夹中创建虚拟环境env2
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ virtualenv env2
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ ls
			env2  manage.py  project  requirement.txt
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ pwd
			/home/tommy/project
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ ls
			env2  manage.py  project  requirement.txt
			source env2//bin/activate  进入到虚拟环境env2中
			tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ source env2//bin/activate
			安装 requirement.txt 中的包
			(env2) tommy@iZ2zeavr5vrs9pwvduqsp4Z:~/project$ pip install -r requirement.txt 
