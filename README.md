# monkey ѹ������android 
## Monkey������
* ���ԵĶ����ΪӦ�ó��������һ���ľ����ԡ�
* Monkey����ʹ�õ��¼���������������ģ����ܽ����Զ��塣
* �ɶ�MonkeyTest�Ķ����¼����������ͣ�Ƶ�ʵȽ������á�
 
## Monkey�Ļ����÷�
* �����﷨���£�
	* $ adb shell monkey [options]
	* �����ָ��options��Monkey�����޷���ģʽ�����������¼����ⷢ�͵���װ��Ŀ�껷���е�ȫ������������һ����Ϊ���͵�������ʾ����������ָ����Ӧ�ó��򣬲����䷢��500��α����¼���
	* $ adb shell monkey -p your.package.name -v 500
## ������־
* ͨ��Android trace�ļ���������ANRʵ������
* system/build.prop ��־�ļ���Ҫ��¼�ֻ�ϵͳ��Ϣ����汾���ͺţ�Ʒ��
* adb logcat ������־�ļ�

## monkey.ini �����ļ�
``` ����
cmd=adb shell monkey -p com.dgm.user --throttle 500 --ignore-timeouts --ignore-crashes   --monitor-native-crashes -v -v
package_name=com.dgm.user
logdir=d:\android
remote_path=d:\android_server
phone_msg_log=d:\android_temp\phone.txt
sum = 100 -
activity = com.dgm.user.SplashActivity
exceptions=['NullPointer','IllegalState','IllegalArgument','ArrayIndexOutOfBounds','RuntimeException','SecurityException'] 
```
- throttle ÿ���¼��ȴ�500����
- sum ��������¼���
- exceptions �쳣���壬���ں�����չ
## �������Ϊ���ӻ�ͼƬ ʹ�õ���matplotlib 
![monkey��־ͼ](img/monkey.png  "monkey��־ͼ")

* ��Ȼ���Կ���־�ļ�

### java�ļ�������д�Ŀ�ָ�����
### monkneytest.py��� 

## 2016-9-3  ������־
* ������(DAL,BLL,MODEL)�ֲ�ķ�ʽ�ع���������

## 2016-9-12 ������־

* monkey���app�����ܲ����������Ͳ�׼ȷ���Ѿ�ȥ��
* ����monkey���ȶ��Թ��ܲ��ԣ����Ա��棺

![monkey���](img/monkey1.png  "monkey���")

![monkey��־](img/log.png  "monkey��־")

* ���Բο��ҵ�[ui�Զ�������ƽ̨](github.com/284772894/appiumn_auto)





