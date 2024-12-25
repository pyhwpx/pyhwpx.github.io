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

<warning>If you delete a user, all their transactions 
    will also be erased from the database.</warning>
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

<i>ideomatic &amp; italic</i>
```

<i>ideomatic & italic</i>

## a

```XML
<a href="Quickstart.md" summary="Show this text in the tooltip">
    Some link
</a>
```

<a href="Quickstart.md" summary="Show this text in the tooltip">Some link</a>

## b

```XML

<b>bold</b>
```

<b>bold</b> and not

## br

```XML
<p>줄바꿈<br/>(break)</p>
```

<p>줄바꿈<br/>(break)</p>

## seealso

## table

<table>
<tr style="header-row">
<td>asdf</td>
<td>zxcv</td>
<td>qwer</td>
</tr>    
<tr>
    <td>First cell in the first row</td>
    <td>Second cell in the first row</td>
    <td>Third cell in the first row</td>
</tr>
</table>

## tabs

탭을 그룹으로 묶어준다.

```XML
<tabs>
    <tab title="Foo">Content of tab Foo</tab>
    <tab title="Bar">Content of tab Bar</tab>
</tabs>
```

<tabs>
    <tab title="Foo">Content of tab Foo</tab>
    <tab title="Bar">Content of tab Bar</tab>
</tabs>

```XML
<tabs>
    <code-block lang="java">Java code</code-block>
    <code-block lang="groovy">Groovy code</code-block>
</tabs>
```

<tabs>
    <code-block lang="java">Java code</code-block>
    <code-block lang="groovy">Groovy code</code-block>
</tabs>

## tip

```XML
<tip>Alternatively, you can change the settings 
    directly in the configuration file.</tip>
```

<tip>Alternatively, you can change the settings directly in the configuration file.</tip>

## note

```XML
<note>
    Use a note for important information that the reader 
    should be aware of, like known issues or limitations.
</note>
```

<note>
    Use a note for important information that the reader should be aware of,
    like known issues or limitations.
</note>

## tldr

```XML
<tldr>
    <p>Shortcut: <shortcut>Ctrl+Space</shortcut></p>
    <p>Configure: 
        <ui-path>
        Settings / Preferences | Editor | Code Completion
    </ui-path>
    </p>
</tldr>
```

<tldr>
    <p>Shortcut: <shortcut>Ctrl+Space</shortcut></p>
    <p>Configure: <ui-path>Settings / Preferences | Editor | Code Completion</ui-path></p>
</tldr>

## tooltip

```XML
<p>Choose your <tooltip term="foo">OS</tooltip>.</p>
```

<p>Choose your <tooltip term="foo">OS</tooltip>.</p>

## ui-path

```XML
<p>From the main menu, select <ui-path>File | New | Project</ui-path>.
</p>
```

<p>From the main menu, select <ui-path>File | New | Project</ui-path>.</p>

## video

```XML
<video src="https://youtu.be/R8QW8s4Ibio"/>
```

<video src="https://youtu.be/R8QW8s4Ibio"/>

## p

```XML
<p id="unique-id">
    Lorem ipsum dolor sit amet, consectetur
    adipiscing elit, sed do eiusmod tempor
    incididunt ut labore et dolore magna
    aliqua.
</p>
```

<p id="unique-id">
    Lorem ipsum dolor sit amet, consectetur
    adipiscing elit, sed do eiusmod tempor
    incididunt ut labore et dolore magna
    aliqua.
</p>
<p>
    Ut enim ad minim veniam, quis nostrud
    exercitation ullamco laboris nisi ut
    aliquip ex ea commodo consequat.
</p>

## inline elements

```XML
<procedure id="example-procedure">
    <step>
        Click <control>OK</control>,
        call <code>doThis()</code>,
        open <path>file.txt</path>,
        select <ui-path>Edit | Copy</ui-path>,
        and stay <emphasis>focused</emphasis>.</step>
</procedure>
```

<procedure id="example-procedure">
    <step>
        Click <control>OK</control>,
        call <code>doThis()</code>,
        open <path>file.txt</path>,
        select <ui-path>Edit | Copy</ui-path>,
        and stay <emphasis>focused</emphasis>.</step>
</procedure>

## chapter

```XML
<chapter title="Example chapter" id="example-chapter-id">
   <p>Some text.</p>
   <chapter title="Subchapter" id="subchapter">
       <p>Some more text.</p>
   </chapter>
</chapter>
```

<chapter title="Example chapter" id="example-chapter-id">
   <p>Some text.</p>
   <chapter title="Subchapter" id="subchapter">
       <p>Some more text.</p>
   </chapter>
</chapter>

## procedure

```XML
<procedure title="Add something" id="procedure-id">
   <p>Before adding something, create it.</p>
   <step>Do this.</step>
   <step>Do that.</step>
   <p>Congratulation! You've added something.</p>
</procedure>
```

<procedure title="Add something" id="procedure-id">
   <p>Before adding something, create it.</p>
   <step>Do this.</step>
   <step>Do that.</step>
   <p>Congratulation! You've added something.</p>
</procedure>

## preview-src

```md
![Alt Text](001.png){ thumbnail="true" preview-src="001.png" }
```

![Alt Text](001.png){ thumbnail="true" preview-src="001.png" }

## link-summary

```XML
<div>
<link-summary rel="some-paragraph"/>
<p id="some-paragraph">Use this paragraph as a link summary</p>
</div>
```

## card-summary

```XML
<card-summary>
    Use card summaries to provide context for cards.
</card-summary>
```

<card-summary>Use card summaries to provide context for cards.</card-summary>

## Math expressions

```XML
<code-block lang="tex">
    \begin{equation}
    x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
    \end{equation}
</code-block>
```

<code-block lang="tex">
    \begin{equation}
    x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
    \end{equation}
</code-block>

