#### 推荐阅读:
#### <https://en.wikipedia.org/wiki/Markdown#Example>
#### <http://www.appinn.com/markdown/>
#### <http://www.jianshu.com/p/1e402922ee32/>

## 推荐使用工具:Ulysses、MWeb、Typora、Marked2、Mou或者直接IntelliJ IDEA安装MarkDown插件

# 以下只做案例汇总,新手请参考推荐阅读

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

# 一级标题 #
## 二级标题 ##
### 三级标题 #######
#### 四级标题 #######
##### 五级标题 #######
###### 六级标题 #################


最高阶标题
====================
第二阶标题
---------------------

#### 无序列表
* 1
* 2
* 3

+ 1
+ 2
+ 3

- 1
- 2
- 3

####有序列表
1. 1
1. 2
1. 3


1. 1
2. 2
3. 3


3. d
1. d
8. d


> 这里是引用

#### 插入链接
[baidu](http://www.baidu.com)
#### 插入图片
![Mou icon](http://www.mouapp.com/Mou_128.png)

*强调*
_强调_
**粗体**
__粗体__

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

http://images.google.com/images?num=30&q=larry+bird

#### &copy;
#### AT&T
#### AT&amp;T

Use the `printf()` function.

``There is a literal backtick (`) here.``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

Please don't use any `<blink>` tags.

`&#8212;` is the decimal-encoded equivalent of `&mdash;`.

    public static void main() {
        System.out.println("right");
    }


#### 分割线:
* * *

***

*****

- - -

---------------------------------------

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.


> ## 这是一个标题。
>
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
>
> 给出一些例子代码：
>
>     return shell_exec("echo $input | $markdown_script");


*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.


*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.


1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

1986. What a great season.

1986\. What a great season.


<http://example.com/>

\*literal asterisks\*



## Spring Framework
The Spring Framework provides a comprehensive programming and configuration
model for modern Java-based enterprise applications -- on any kind of deployment
platform. A key element of Spring is infrastructural support at the application
level: Spring focuses on the "plumbing" of enterprise applications so that teams
can focus on application-level business logic, without unnecessary ties to
specific deployment environments.

The framework also serves as the foundation for [Spring Integration][], [Spring Batch][]
and the rest of the Spring [family of projects][]. Browse the repositories under
the [Spring organization][] on GitHub for a full list.

## Code of Conduct
This project adheres to the Contributor Covenant [code of conduct](CODE_OF_CONDUCT.adoc).
By participating, you  are expected to uphold this code. Please report unacceptable behavior to spring-code-of-conduct@pivotal.io.

## Downloading Artifacts
See [downloading Spring artifacts][] for Maven repository information. Unable to
use Maven or other transitive dependency management tools?
See [building a distribution with dependencies][].

## Documentation
See the current [Javadoc][] and [reference docs][].

## Getting Support
Check out the [spring][spring tags] tags on [Stack Overflow][]. [Commercial support][]
is available too.

## Issue Tracking
Report issues via the [Spring Framework JIRA][]. Understand our issue management
process by reading about [the lifecycle of an issue][]. Think you've found a
bug? Please consider submitting a reproduction project via the
[spring-framework-issues][] GitHub repository. The [readme][] there provides
simple step-by-step instructions.

## Building from Source
The Spring Framework uses a [Gradle][]-based build system. In the instructions
below, [`./gradlew`][] is invoked from the root of the source tree and serves as
a cross-platform, self-contained bootstrap mechanism for the build.

### Prerequisites

[Git][] and [JDK 8 update 20 or later][JDK8 build]

Be sure that your `JAVA_HOME` environment variable points to the `jdk1.8.0` folder
extracted from the JDK download.

### Check out sources
`git clone git@github.com:spring-projects/spring-framework.git`

### Import sources into your IDE
Run `./import-into-eclipse.sh` or read `import-into-idea.md` as appropriate.
> **Note:** Per the prerequisites above, ensure that you have JDK 8 configured properly in your IDE.

### Install all spring-\* jars into your local Maven cache
`./gradlew install`

### Compile and test; build all jars, distribution zips, and docs
`./gradlew build`

... and discover more commands with `./gradlew tasks`. See also the [Gradle
build and release FAQ][].

## Contributing
[Pull requests][] are welcome; see the [contributor guidelines][] for details.

## Staying in Touch
Follow [@SpringCentral][] as well as [@SpringFramework][] and its [team members][]
on Twitter. In-depth articles can be found at [The Spring Blog][], and releases
are announced via our [news feed][].

## License
The Spring Framework is released under version 2.0 of the [Apache License][].

[Spring Integration]: https://github.com/spring-projects/spring-integration
[Spring Batch]: https://github.com/spring-projects/spring-batch
[family of projects]: http://spring.io/projects
[Spring organization]: https://github.com/spring-projects
[downloading Spring artifacts]: https://github.com/spring-projects/spring-framework/wiki/Downloading-Spring-artifacts
[building a distribution with dependencies]: https://github.com/spring-projects/spring-framework/wiki/Building-a-distribution-with-dependencies
[Javadoc]: http://docs.spring.io/spring-framework/docs/current/javadoc-api/
[reference docs]: http://docs.spring.io/spring-framework/docs/current/spring-framework-reference/
[spring tags]: http://spring.io/questions
[Stack Overflow]: http://stackoverflow.com/faq
[Commercial support]: http://spring.io/services
[Spring Framework JIRA]: https://jira.spring.io/browse/SPR
[the lifecycle of an issue]: https://github.com/spring-projects/spring-framework/wiki/The-Lifecycle-of-an-Issue
[spring-framework-issues]: https://github.com/spring-projects/spring-framework-issues#readme
[readme]: https://github.com/spring-projects/spring-framework-issues#readme
[Gradle]: http://gradle.org
[`./gradlew`]: http://vimeo.com/34436402
[Git]: http://help.github.com/set-up-git-redirect
[JDK8 build]: http://www.oracle.com/technetwork/java/javase/downloads
[Gradle build and release FAQ]: https://github.com/spring-projects/spring-framework/wiki/Gradle-build-and-release-FAQ
[Pull requests]: http://help.github.com/send-pull-requests
[contributor guidelines]: https://github.com/spring-projects/spring-framework/blob/master/CONTRIBUTING.md
[@SpringFramework]: https://twitter.com/springframework
[@SpringCentral]: https://twitter.com/springcentral
[team members]: https://twitter.com/springframework/lists/team/members
[The Spring Blog]: http://spring.io/blog/
[news feed]: http://spring.io/blog/category/news
[Apache License]: http://www.apache.org/licenses/LICENSE-2.0


<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=#0099ff size=7 face="黑体">color=#0099ff size=72 face="黑体"</font>
<font color=#00ffff size=72>color=#00ffff</font>
<font color=gray size=72>color=gray</font>
        
        Size：规定文本的尺寸大小。可能的值：从 1 到 7 的数字。浏览器默认值是 3。





