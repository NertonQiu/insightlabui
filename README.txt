3.����Git
��1�� �����ڱ��ش���ssh key��
    $ ssh-keygen -t rsa -C "your_email@youremail.com"
 �����your_email@youremail.com��Ϊ������䣬֮���Ҫ��ȷ��·�����������룬������ʹ��Ĭ�ϵ�һ·�س����С��ɹ��Ļ�����~/������.ssh�ļ��У���ȥ����id_rsa.pub�����������key���ص�github������Account Settings�����ѡ��SSH Keys��Add SSH Key,title����ճ��key��

��2��Ϊ����֤�Ƿ�ɹ�����git bash�����룺
    $ ssh -T git@github.com 
 ����ǵ�һ�εĻ���ʾ�Ƿ�continue������yes�ͻῴ����You��ve successfully authenticated, but GitHub does not provide shell access ����ͱ�ʾ�ѳɹ�����github��
��3������������Ҫ���ľ��ǰѱ��زֿ⴫��github��ȥ���ڴ�֮ǰ����Ҫ����username��email����Ϊgithubÿ��commit�����¼���ǡ�
 $ git config --global user.name "your name" 
 $ git config --global user.name "your name"$ git config --global user.email "your_email@youremail.com"
 ��4������Ҫ�ϴ��Ĳֿ⣬�Ҽ�git bash�����Զ�̵�ַ��
  $ git remote add origin git@github.com:yourName/yourRepo.git
 �����yourName��yourRepo��ʾ����github���û����͸ղ��½��Ĳֿ⣬����֮�����.git����config���������һ��remote ��origin�����ݣ�����Ǹղ���ӵ�Զ�̵�ַ��Ҳ����ֱ���޸�config������Զ�̵�ַ��

4.�ύ���ϴ�
  ��1���������ڱ��زֿ������һЩ�ļ�������README��
   $ git add README
   $ git commit -m "first commit" 
   ��2���ϴ���github��
   $ git push origin master 
   git push����Ὣ���زֿ����͵�Զ�̷�������
   git pull�������෴��
   �޸�������ʹ��git status���Բ鿴�ļ��Ĳ��ʹ��git add ���Ҫcommit���ļ���Ҳ������git add -i����������ļ���֮��git commit�ύ�����޸ģ�git push�ϴ���github��