# Android Killer

> Attention: This project uses charset GB2312 for compatibly reason.
>
> ע�⣺���ڼ�����ԭ�򣬱���Ŀʹ�� GB2312 �ַ�����

���ϲ��������������� Android �����빤�� ���� Android Killer��������ս 20 �꣡

˼·�ͷ������Դ���[��ҹ�ǳ� 2012](https://www.52pojie.cn/home.php?mod=space&uid=571540&do=profile&from=space) �� [AndroidKiller ��װ�����ü�ʹ�ý̳�](https://www.52pojie.cn/thread-726176-1-1.html)��

���߱Ͼ������ˣ������ǽ��滹�ǹ����϶��������⣬С���ڴ˻����Ƽ��͹ٳ��� JEB Decompiler 3 ������ά���� Android �����빤�ߡ�

## ʹ��

���[�˴�](../../archive/refs/heads/main.zip)��������ѹ��������ѹ���Ŀ¼��˫������ AndroidKiller.exe ���ɡ�

Android Killer ����ϸʹ�ý̳���[�ο�����](https://blog.csdn.net/yiran1919/article/details/132760445)������������

**ע�����ʹ�ñ�����ǰ������Ҫ�ڵ������ú� Java ���л�����**

## ��������

- `bin/`
  - ���� adb �� busybox���汾���ˣ����þ��У�������˵ ?��
  - ���� apktool.jar �� v2.11.1
  - ���� dex2jar �� v2.4
  - ���� Android Killer ���õ� jd-gui��ʹ���Լ���д���м���� [android-killer-jadx-gui-support](../../../android-killer-jadx-gui-support) ������ת���� jadx-gui
- `tools/`
  - ��� [ApkScan PKID](http://www.legendsec.org/1888.html) ��ǹ��ߣ����������Զ��Ч���޷���֤������Ѱ�����������
  - ��� [InjectLog](https://www.52pojie.cn/thread-743758-1-1.html) ��־���ߣ��ּ� [Android Ӧ�����򡪡��������������֮������](https://blog.csdn.net/charlessimonyi/article/details/52027563)
  - ��� jadx-gui ������ jre �汾�������� v1.4.7��GitHub �ϴ����ļ�������� 100MB��v1.5.0+ �汾���ޣ������и�����Ҫ���볢��[���и���](#jadx-gui-���·���)��

## ���и���

### apktool ���·���

1. �� [apktool ����ҳ��](https://github.com/iBotPeaches/Apktool/releases) �������°�� `apktool_x.x.x.jar`
2. ������ `bin/apktool/apktool/` Ŀ¼�£��� **Android Killer** ��ҳ�� **Android** �˵����� **APKTOOL ������**��������صİ汾������ΪĬ��

   ![չʾ](docs/images/image1.png)
   ![չʾ](docs/images/image2.png)

### dex2jar ���·���

1. �� [dex2jar ����ҳ��](https://github.com/pxb1988/dex2jar/releases) �������°�� `dex-tools-xxx.zip`���ɰ���Ϊ `dex2jar-xxx.zip`��
2. ��� `bin/dex2jar/` Ŀ¼���ļ��������صõ���ѹ��������ȫ����ѹ������Ŀ¼

### jadx-gui ���·���

1. �� [jadx ���ؽ���](https://github.com/skylot/jadx/releases) �������°�� `jadx-gui-x.x.x-win.zip`���ɰ�Ϊ `jadx-gui-x.x.x-no-jre.exe`��
2. ��ѹ�������ݽ�ѹ�� `tools/JadxGui/` Ŀ¼�£������� `jadx-gui-x.x.x.exe` Ϊ `jadx-gui.exe`�����Ǿɰ棨�ɰ�ֱ����������ִ�г��򣬺󸲸Ǽ��ɣ�

## ע������ & һЩ����

- ����Ӧ��ʱ�빴ѡ AndroidKiller ǩ�������������� apk �ļ����ʲ�������ʹ��
- �����װ���� "Failure [INSTALL_FAILED_INVALID_APK: Failed to extract native libraries, res=-2]"�� �뽫 `AndroidManifest.xml` �ļ��е� `extractNativeLibs=false` �޸�Ϊ `extractNativeLibs=true`���ٴγ���
