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
File[] files = new File[10];
File file1 = new File("");
File file1 = new File("");
List<File> fileList = new ArrayList<File>();

try {
	//key value
	params.put("images[]", files);	
	params.put("files[]", file1, file2);
	params.put("filelist[]", fileList);
} catch (FileNotFoundException e) {
	e.printStackTrace();
}
```

RequestParams Method �߰� ����
---------
```
put(String key, File... files)
put(String key, List<File> fileList)
put(String key, String customFileName, File... files)
put(String key, String customFileName, List<File> fileList)
put(String key, File[] files, String contentType)
put(String key, List<File> fileList, String contentType)
```

���� ���� �ذ���
---------
POST,GET ���۽� No valid URI scheme was provided ���� �߻���

setURLEncodingEnabled �� ��Ȱ��ȭ ���ּ���.

(URL ���ڵ��� �ڵ� Ȱ��ȭ �Ǿ� �ֱ� ������ ���� ���� �� �ֽ��ϴ�.)

```
AsyncHttpClient client = new AsyncHttpClient();
client.setURLEncodingEnabled(false);
```


������Ʈ ����
---------
[2014-09-29]
File Array, File List ���� �߰�.

[2014-09-28]
1. ��Ƽ ���� ���ε� �߰�.


License
---------
Apache License 2.0