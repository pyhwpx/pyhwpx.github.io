# Writerside Components

## 파일을 다운받게 하는 방법

프로젝트 루트의 `resources` 디렉토리에 파일을 넣어 두고, 본문에 마크업을 입력한다.

<tabs>
<tab title="결과">
Donwload <resource src="sample.hwp">file</resource> and open it.
</tab>
<tab title="코드">
<code-block lang="XML">
Donwload &lt;resource src="sample.hwp"/&gt; and open it.
</code-block>
</tab>
</tabs>

writerside의 semantic elements는 현재 총 77개다.

## warning

```XML
<warning>If you delete a user, all their transactions will also be erased from the database.</warning>
```

<warning>If you delete a user, all their transactions will also be erased from the database.</warning>

## resource

```XML
<resource src="sample.hwp">샘플문서 다운로드</resource>
```

<resource src="sample.hwp">샘플문서 다운로드</resource>

## img

```XML
<img src="001.png" alt="001.png"/>
```

<img src="001.png" alt="001.png"/>

## i

```XML
<i>ideomatic & italic</i>
```

<i>ideomatic & italic</i>

## a

```XML
<a href="Quickstart.md">quickstart</a>
```

<a href="Quickstart.md">quickstart</a>

## api-doc : pass

## api-endpoint : pass

## api-schema : pass

## b

```XML
<b>bold</b>
```

<b>bold</b> and not

## br

```XML
줄바꿈<br></br>(break)
```

줄바꿈<br></br>(break)

