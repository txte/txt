$ pwd  ����
$ git init ��ʼ��
$ git add readme.txt   ���ļ���ӵ��ֿ�(������stage)
$ git commit -m "wrote a readme file"  ���ļ��ύ���ֿ⡰ע�͡� -m����������Ǳ����ύ��˵������֧master��
                                                           1 file changed��1���ļ����Ķ�����������ӵ�readme.txt�ļ�����
                                                           2 insertions���������������ݣ�readme.txt���������ݣ���
                                                           ��Ҫ�ύ���ļ��޸�ͨͨ�ŵ��ݴ�����Ȼ��һ�����ύ�ݴ����������޸ġ�
$ git status �������������ʱ�����ղֿ⵱ǰ��״̬��readme.txt���޸Ĺ��ˣ�����û��׼���ύ���޸ġ�

####����
$ git checkout -- readme.txt  ���Գ������������޸�,������ļ��ص����һ��git commit��git addʱ��״̬
$ git reset HEAD readme.txt   ���ݴ������޸ĳ�������unstage�������·Żع�������

####ɾ��
$ git rm test.txt   �Ӱ汾����ɾ�����ļ����Ǿ�������git rmɾ��������git commit��

$ git diff �������޸���ʲô���ݣ��Ƚϵ��ǹ������ļ����ݴ����ļ�������
$ git diff --cached �Ƚϵ����ݴ������ļ���ֿ��֧��ϴ�git commit ������ݣ�������
$ git diff HEAD -- readme.txt������Բ鿴�������Ͱ汾���������°汾������

####�汾����
$ git log  �ύ��ʷ
$ git log --pretty=oneline �汾��
$ git reset --hard HEAD^ �ϸ��汾   HEAD~10�汾��  HEADָ��İ汾���ǵ�ǰ�汾
$ git reset --hard 1094a    ���Ի�ԭ�汾  1094a
$ git reflog �鿴������ʷ���Ա�ȷ��Ҫ�ص�δ�����ĸ��汾��

####Զ�ֿ̲�GitHub
$ git remote add origin git@github.com:txte/txt.git    
 Զ�̿�����־���origin
$ git push -u origin master   ���ؿ�������������͵�Զ�̿��ϣ� -u��������ѱ��ص�master��֧�������͵�Զ���µ�master��֧�����ص�master��֧��Զ�̵�master��֧��������
$ git push origin master  �Ժ�����ͻ�����ȡʱ�Ϳ��Լ�����
