����ʹ��git��GitHub�ϴ����ֿ����ϸ����

ʹ��GitHub�ֿ���Ա��
a.GitHub��
	1> ע���˻��Լ������ֿ�

b.����
http://www.runoob.com/w3cnote/git-guide.html

	1> ��װgit �� openssh�����ش���ssh key
		$ ssh-keygen -t rsa -C "your_email@youremail.com"
		�����your_email@youremail.com��Ϊ����github��ע������䣬֮���Ҫ��ȷ��·�����������룬������ʹ��Ĭ�ϵ�һ·�س����С��ɹ��Ļ�����~/������.ssh�ļ��У���ȥ����id_rsa.pub�����������key��
		�ص�github�ϣ����� Account Settings���˻����ã������ѡ��SSH Keys��Add SSH Key,title����ճ��������������ɵ�key��
	
	2> ��֤�Ƿ�ɹ�����git bash�����룺
		$ ssh -T git@github.com

	3> ����username��email����ΪGitHubÿ��commit�����¼����
		$ git config --global user.name "your name"
		$ git config --global user.email "your_email@youremail.com"
		
	4> clone�ֿ�
		$ git clone git@github.com:aislingwang/githubTest.git
		
	5> �޸ĺ��ύ
	6> ����ļ����ύ
		
		
		
/////////////////////////////////////////////////////////////////////////////////////////////////////////////



		
�����ֿ���Ա��
a.GitHub��
	1> ע���˻��Լ������ֿ�
		github������ַ��https://github.com/
		Create a New Repository��������ƺ�Create��֮������һЩ�ֿ��������Ϣ
	
b.����
http://www.runoob.com/w3cnote/git-guide.html

	1> ��װgit �� openssh�����ش���ssh key
		$ ssh-keygen -t rsa -C "your_email@youremail.com"
		�����your_email@youremail.com��Ϊ����github��ע������䣬֮���Ҫ��ȷ��·�����������룬������ʹ��Ĭ�ϵ�һ·�س����С��ɹ��Ļ�����~/������.ssh�ļ��У���ȥ����id_rsa.pub�����������key��
		�ص�github�ϣ����� Account Settings���˻����ã������ѡ��SSH Keys��Add SSH Key,title����ճ��������������ɵ�key��
	
	2> ��֤�Ƿ�ɹ�����git bash�����룺
		$ ssh -T git@github.com
	
	3>���Զ�̵�ַ��
		$ git remote add origin git@github.com:yourName/yourRepo.git
		�����yourName��yourRepo��ʾ����github���û����͸ղ��½��Ĳֿ⣬����֮�����.git����config���������һ��remote "origin"���ݣ�����Ǹղ���ӵ�Զ�̵�ַ��Ҳ����ֱ���޸�config������Զ�̵�ַ��
		�������ļ��У��򿪣�Ȼ��ִ�� git init �Դ����µ� git �ֿ⡣
	
	4> ����username��email����ΪGitHubÿ��commit�����¼����
		$ git config --global user.name "your name"
		$ git config --global user.email "your_email@youremail.com"
	
	5> ����ļ����ύ��Զ�ֿ̲⣬���͵�Զ��master��֧
		$ git add .
		$ git commit -m ��first commit��
		$ git push -u origin master
	
	6> ���˹�ͬ����
		http://blog.csdn.net/song_shui_lin/article/details/52685780