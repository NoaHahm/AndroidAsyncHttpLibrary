AndroidAysncHttpLibrary
=======================

�ȵ���̵� AysncHttp ���¼ҽ� ���̺귯�� (Loopj) 1.4.7 ������ ������ ���� �Դϴ�.

AysncHttp ���¼ҽ� ���̺귯���� ���� ���ϸ� ���ε尡 �����մϴ�. 

����, �� ���¼ҽ� ������Ʈ�� ����Ͻø� ���� ���� ���ε� �Ӹ� �ƴ϶�,

���� ���ϱ��� ���ε� �Ͻ� �� �ֽ��ϴ�.

(��Ȯ�� ������� ����Ȩ�������� �������ּ���.)



���� Ȩ������ : http://loopj.com/android-async-http

�����
---------
POST ���۽� ���� File �Ӹ� �ƴ϶� File Array ���·� ���� ���� ������ �����մϴ�.

```
RequestParams params = new RequestParams();

try {
	params.put("images[]", file);
} catch (FileNotFoundException e) {
	e.printStackTrace();
}
```


���� ���� �ذ���
---------
POST,GET ���۽� No valid URI scheme was provided ���� �߻���

setURLEncodingEnabled �� ��Ȱ��ȭ ���ּ���.

(URL ���ڵ��� �ڵ� Ȱ��ȭ �Ǿ� �ֱ� ������ ���� ���� �� �ֽ��ϴ�.)


������Ʈ ����
---------
1. ��Ƽ ���� ���ε� �߰�.


License
---------
Apache License 2.0