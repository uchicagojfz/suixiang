
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="zh-CN">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=gb18030" />
<meta name="generator" content="Python script by program.think@gmail.com" />
<meta name="provider" content="program-think.blogspot.com" />
<link type="text/css" rel="stylesheet" href="../../css/program-think.css" />
<title>C++�Ŀ���ֲ�ԺͿ�ƽ̨����[6]�����߳� - �������Ĳ���</title>
</head>
<body>
<div id="main" style="width:100%;">
<h1><a href="../../index.md" title="�ص���ҳ">C++�Ŀ���ֲ�ԺͿ�ƽ̨����[6]�����߳�</a></h1>
<div class="post-info"><span class="date-header">2009-04-03</span><a href="../../tags/E7BC96E7A88B.C.md" class="tag">���.C</a> <a href="../../tags/E7BC96E7A88B.md" class="tag">���</a> <a href="../../tags/E7BC96E7A88B.E5A49AE7BABFE7A88B.md" class="tag">���.���߳�</a> </div>
<hr>
<div class="post">
�������һ������д�����ӱȽ��ӣ����±�ϵ���ֺþ�û�����ˡ�������������������д����ˣ�������е�塣����Ͻ��Ѷ��߳�ƪ���ϡ�<a href="../../2009/02/cxx-cross-platform-develop-5-os.md" target="_blank">�ϴ��Ĳ���ϵͳ</a>��ʱ�����ں�OS�йصĻ���Ƚ����飬�����Ӱ�˵��һ��ѡ���ʱһ��ƪ���е㳤���ͰѶ���̺Ͷ��̵߳Ĳ��ָ����������ˡ�<!--program-think--><br /><br />������<b>������</b><br />���������C���п�ѡ��<br />��������˵һ���ܻ��������⣺����C���п⣨������CRT��C Run-Time�������á�������������ô�ͼ������⣬����Χ�кü����˶�������ط��Թ��������Ի��ǽ�һ�¡�<br />�����󲿷�C++�����������Դ���CRT�����ܻ���ֹһ������ĳЩ�������Դ���CRT���ܻ�����̵߳�֧�ַ�Ϊ���߳�CRT�Ͷ��߳�CRT���ࡣ����Ҫ���ж��߳̿�����ʱ�򣬱�����ȷ����ص�C++������Ŀʹ�õ��Ƕ��̵߳�CRT����������ú��ѿ���<br />�������䵱��ʹ��Visual C++����������Ŀ������ҪС�ġ�����½��Ĺ�����Ŀ�ǲ���MFC�ģ�����Console���̺�Win32���̣����ǹ��̵�Ĭ�����û���ʹ�á����߳�CRT��������ͼ��ʾ��<br /><center><img src="../../images/2009/04/OgAAAJJFds5n7h9uopMdDYFXoT_exZc9kByApTXfK34KyHSvIsdZrYIRK6H-hqsbUWqfIQIXtSD7SrpRxWC4SoM7SbEA15jOjKhsWykOsXmpMQ4TVasMh_oy3ng9"  alt="����ͼ���뷭ǽ"/></center><br />����������Ż�ѡ��<br />�������Ż�ѡ�����һ���ܹؼ��ı�������ػ��⡣��Щ�������ṩ�ųƺ�ţX���Ż�ѡ�����ĳЩ�Ż�ѡ����ܻ���Ǳ�ڵķ��ա������������������Ŵ���ִ��ָ���˳�򣬴Ӷ����³������ϵ��߳̾�̬���⣨Race Condition����ϸ���Ϳ���<a href="http://en.wikipedia.org/wiki/Race_condition#Computing" target="_blank" rel="nofollow">����</a>��������δ��ͬѧ�ڡ�<a href="http://blog.csdn.net/pongba/archive/2007/06/20/1659952.aspx" target="_blank" rel="nofollow">C++���߳��ڴ�ģ��</a>������˼������͵����ӣ���������ȥ��һ�ơ�<br />��������ֻʹ�ñ�����������ٶ��Ż�ѡ��ɡ�������Щ���ڵ��Ż�ѡ����ӵ�Ч��δ�����ԣ�����Ǳ�ڵķ��ղ�С��ʵ�ڲ�ֵ��ð�ա�<br />������GCCΪ����������<b>-O2</b>ѡ��ɣ���ʵ<b>-O2</b>��һ��ѡ��ļ��ϣ���û��Ҫð����<b>-O3</b>���������кܳ�������ɣ�������<b>-O2</b>��<b>-O3</b>֮�⣬GCC����һ���磨�������ϰٸ����������Ż�ѡ��������ͼ�õ��е�ĳ��ѡ�һ��Ҫ�Ȱ��������ԡ����ܵĸ����ö��������������������֪����ô���ġ�<br /><br />������<b>�߳̿��ѡ��</b><br />�������ڵ�ǰ��C++ 03��׼����û���漰�߳���ص����ݣ���ʹ����C++ 0x�������̵߳ı�׼�⣬���������̵�֧���ڶ�����Ҳδ��ȫ�棩��������δ���ܳ���һ��ʱ�䣬��ƽ̨�Ķ��߳�֧�ֻ���Ҫ�����������⡣�����߳̿��ѡ���Ǵ�����Ҫ��������½���һ�¼���֪���Ŀ�ƽ̨�߳̿⡣<br />������<a href="http://www.cs.wustl.edu/%7Eschmidt/ACE.md" target="_blank" rel="nofollow">ACE</a><br />������˵һ��ACE�����ʷ�ƾõĿ⡣�����֮ǰ��δ�Ӵ��������ȿ���<a href="http://en.wikipedia.org/wiki/Adaptive_Communication_Environment" target="_blank" rel="nofollow">����</a>��ɨä����ACE��ȫ�ƣ�Adaptive Communication Environment����������Ӧ�����ԡ�ͨѶ��Ϊ��ҵ������ACE�ԡ����̡߳������ҵ��֧�ֻ��Ƿǳ�ȫ��ģ����绥������ACE_Mutex��������������ACE_Condition�����ź�����ACE_Semaphore����դ����ACE_Barrier����ԭ�Ӳ�����ACE_Atomic_Op���ȵȡ���ĳЩ���ͱ���ACE_Mutex��ϸ��Ϊ�̶߳�д����ACE_RW_Thread_Mutex�����̵߳ݹ�����ACE_Recursive_Thread_Mutex���ȵȡ�<br />��������֧�ֺ�ȫ�棬ACE������һ�������Ե��ŵ㣬���ǶԸ��ֲ���ϵͳƽ̨�����Դ��ı�����֧�ֺܺá�����һЩ��ʽ�ı�����������VC6������Ҳ�ܹ�֧�֣��˴���˵��<b>֧��</b>���������ܱ���ͨ��������Ҫ���ȶ����У�������ŵ���ڿ�ƽ̨���������൱�൱�����ԡ�<br />������ȱ��������ACE��������ͷ���磨����������;�ʮ������ڣ����ǻ���ܶ�C++�������Զ���û�������������������ˣ������Ըо�ACE�����ķ��Ƚ�������Զ����boost��ôʱ��ǰ����<br />������<a href="http://www.boost.org/doc/html/thread.md" target="_blank" rel="nofollow">boost::thread</a><br />����boost::thread���ú�ACE�γ��������ա�������ò�ƴ�boost 1.32�汾��ʼ���룬��ͷ��ACE�̡�����������boost��һ���ţ��֧�֣���չ��������ġ���Ŀǰ��boost 1.38�汾��Ҳ�ܹ�֧�����������ˣ������ƺ�ûACE�ࣩ�����ںܶ�C++��׼ίԱ��ĳ�Ա�Ƽ���boost�����У�����ʱ������ƣ�boost::thread�ս���ΪC++�̵߳�����֮�ǣ�ǰ;��������<br />����boost::thread��ȱ�����֧�ֵı����������࣬������һЩ<b>��ʽ</b>���������ܶ�boost���ӿⶼ�д����⣬�����Ϊ����һЩ�߼���ģ���﷨��������ڿ�ƽ̨����һ���Ƚ����Ե����⡣<br />������<a href="http://www.wxwidgets.org/" target="_blank" rel="nofollow">wxWidgets</a>��<a href="http://www.qtsoftware.com/" target="_blank" rel="nofollow">QT</a><br />����wxWidgets��QT����GUI����⣬��������Ҳ�����úͶ��̵߳�֧�֡�wxWidgets�̵߳ļ����Կ���<a href="http://docs.wxwidgets.org/trunk/overview_thread.md" target="_blank" rel="nofollow">����</a>��������QT�̵߳ļ����Կ���<a href="http://doc.trolltech.com/4.0/threads.md" target="_blank" rel="nofollow">����</a>��������������̵߳�֧�ֲ�࣬���ṩ������mutex��condition��semaphore�ȳ��õĻ��ơ���������û��ACE�ḻ��<br />������<b>���Ȩ��</b><br />�������ڿ���GUI�������Ѿ�������wxWidgets����QT���������ֱ�����������õ��߳̿⣨ǰ������ֻ�õ��������̹߳��ܣ��������������õ��߳̿⣬�������ӵ�������һ����Ҫĳ�߼����̹߳��ܣ��ǵÿ����滻��boost::thread��ACE��<br />��������boost::thread��ACE��ȡ�ᣬ��Ҫ�ÿ������������ˡ������Ҫ֧�ֵ�ƽ̨ͦ��ͦ�ӣ��ǽ���ѡ��ACE���������ϱ�������֧�ֵ����⡣�����ֻ��Ҫ֧����������������ƽ̨������Windows��Linux��Mac�����ǽ�����boost::thread���Ͼ���������ϵͳ�ϵı���������boost��֧�ֻ������õġ�<br /><br />������<b>����ϵ�ע������</b><br />������ʵ���߳̿�������Ҫע��ĵط�ͦ��ģ���ֻ�ܴ����м���ӡ��Ƚ����ע�����<br />���������<b>volatile</b><br />����˵�����̱߳�̿������������壬�ǾͲ��ò��ᵽ<b>volatile</b>�ؼ��֡����������������˽⣬�ȿ���<a href="http://en.wikipedia.org/wiki/Volatile_variable" target="_blank" rel="nofollow">����</a>��ɨäһ�¡�����C++ 98��C++ 03��׼��û�ж�����̵߳��ڴ�ģ�ͣ�����׼��Ҳ��<b>volatile</b>���߳�մ����ߡ��������C++���������൱��Ŀ�ˮ��������<b>volatile</b>���ϣ������в���C++��ţ�Ŀ�ˮ�����м��ڴˣ�������Ͳ��ٶ������ˡ��Ƽ�������ţ�����£�<a href="http://en.wikipedia.org/wiki/Andrei_Alexandrescu" target="_blank" rel="nofollow">Andrei Alexandrescu</a>�����¡�<a href="http://www.ddj.com/cpp/184403766" target="_blank" rel="nofollow">����</a>��������Hans Boehm�����¡�<a href="http://www.hpl.hp.com/personal/Hans_Boehm/c++mm/user-faq.md" target="_blank" rel="nofollow">����</a>���͡�<a href="http://www.open-std.org/JTC1/sc22/wg21/docs/papers/2006/n2016.md" target="_blank" rel="nofollow">����</a>���������Ը���ȥ�ݶ�һ�¡�<br />���������ԭ�Ӳ���<br />������Щͬѧ��֪������̵߳�<b>����д</b>��Ҫ������ȴ��֪�����<b>��</b>����<b>д</b>Ҳ��Ҫ������������ĳ������int nCount = 0x01020304���ڲ���״̬�£�һ��д�߳�ȥ�޸�����ֵnCount = 0x05060708����һ�����߳�ȥ��ȡ��ֵ����ô���߳���û�п��ܶ�ȡ��һ���������ģ�����0x05060304��������<br />���������Ƿ񻵵���ȡ���ڶ�nCount�Ķ���д�Ƿ�����ԭ�Ӳ���������������ںܶ�Ӳ����ص������ˣ�����CPU�����͡�CPU���ֳ����ڴ������ֽ����ȣ�����ĳЩ����£�ȷʵ���ܳ������ݻ�����<br />���������������۵��ǿ�ƽ̨�Ŀ����������ý�����Ĵ������ɶ����Ӳ��������ִ�С������ڴ������������ʱ�򣬻���Ҫ�õ��������ṩ��ԭ�Ӳ�����/����������ACE��Atomic_Op����ȷ����ȫ��<br />��������ڶ��������<br />������֮ǰ��ϵ�����ӡ�<a href="../../2009/02/cxx-object-destroy-overview.md" target="_blank">C++��������ô���ģ�</a>�����棬�Ѿ��ֱ������Win32ƽ̨��Posixƽ̨���̵߳�<b>��</b>��Ȼ�������⡣��������������ƽ̨���߳̿�ײ㻹��Ҫ���ò���ϵͳ�Դ����߳�API�����Դ�������Ҫ�����Ŭ��ȷ��<b>����</b>�̶߳��ܹ���Ȼ������<br /><br />��������Ļ�����ĵ������һ���Ķ���̵Ļ��⡣<div class="blogger-post-footer">
</div>
<hr>
<div class="copyright">
<h4>��Ȩ����</h4>
���������е�ԭ�����£����߽Ա�����Ȩ��ת�ر�����������������ֱ������������Գ�������ʽע������<a href="mailto:program.think@gmail.com">�������</a>�ͱ���ԭʼ��ַ��<br>
<a href="/2009/04/cxx-cross-platform-develop-6-thread.md">2009/04/cxx-cross-platform-develop-6-thread.md</a>
</div>
</div>
</body>
</html>