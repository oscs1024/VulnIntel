# Fastjson 1.2.68-1.2.83远程代码执行漏洞 (MPS-1hjz-nqtx)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>反序列化</td>
            <td><strong>发现时间</strong></td>
            <td>2026-07-21</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-1hjz-nqtx">MPS-1hjz-nqtx</a></td>
            <td><strong>CVE编号</strong></td>
            <td>-</td>
            <td><strong>漏洞影响广度</strong></td>
            <td>广</td>
        </tr>
        </tbody>
    </table>
</figure>


<figure class="wp-block-table">
    <h1 class="wp-block-heading">漏洞危害</h1>
    <table>
        <tbody>
        <tr>
            <td><strong>OSCS 描述</strong></td>
        </tr>
        <tr>
            <td>Fastjson 是阿里巴巴开源的 Java 语言 JSON 解析库，广泛用于实现 JSON 与 Java 对象之间的序列化和反序列化。
Fastjson 1.x 在 autoType 关闭 时，仍会根据 JSON 中的 @type 去读取对应 class 资源，判断是否带有 @JSONType 注解；若有，则仍会 loadClass。当运行环境使用会把资源名当 URL 打开的 ClassLoader（典型为 Spring Boot FatJar 的 LaunchedURLClassLoader）时，攻击者可将 @type 伪造成 jar:http://... 形式，诱导应用从攻击者服务器下载恶意 class 并初始化，从而在 静态初始化块 中执行任意代码。该路径不依赖目标 Classpath 上预置的第三方gadget。
注意：在 spring boot加嵌入式 Tomcat 的普通请求线程且未 set DefaultClassLoader为 LaunchedURLClassLoader的情况下（一般写代码都不会特意设置defaultClassLoader为 LaunchedURLClassLoader），HTTP 请求里 Fastjson会走嵌入式tomcat的TomcatEmbeddedWebappClassLoader，导致只能远程拉jar，不能执行jar里的恶意代码，不能实现rce。
此外目前其它已验证的风险场景为Fastjson 在默认 AutoType 关闭时，若业务使用 JSON.parseObject(body, Dto.class) 且 Dto 含危险字段类型（如 javax.swing.UIDefaults.LazyValue、XMLDecoder 等），攻击者可通过JDK内置链利用，实现远程代码执行。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-1hjz-nqtx">https://www.oscs1024.com/hd/MPS-1hjz-nqtx</a></em>
            </td>
        </tr>
        </tbody>
    </table>
</figure>


<figure class="wp-block-table alignleft">
    <h1 class="wp-block-heading">影响范围及处置方案</h1>
    <h2 class="wp-block-heading"><strong>OSCS</strong> <strong>平台影响范围和处置方案</strong></h2>
    <table>
        <tbody>
        <tr>
            <td>影响范围</td>
            <td>处置方式</td>
            <td>处置方法</td>
        </tr>
        <tr><td rowspan="1">com.alibaba:fastjson [1.2.68,1.2.83_noneautotype)</td><td>缓解措施</td><td>启用 SafeMode或者迁移至 Fastjson 2.x</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-1hjz-nqtx">https://www.oscs1024.com/hd/MPS-1hjz-nqtx</a></em></td>
        </tr>
        </tbody>
    </table>
</figure>


<figure class="wp-block-table">
    <h1 class="wp-block-heading">排查方式</h1>
    <table>
        <tbody>
        <tr>
            <td><strong>方式1：使用漏洞检测CLI工具来排查</strong><em>使用文档：<a
                    href="https://www.murphysec.com/docs/faqs/integration/cli.html">https://www.murphysec.com/docs/faqs/integration/cli.html</a></em>
            </td>
        </tr>
        <tr>
            <td><strong>方式2：使用漏洞检测IDEA插件排查</strong><em>使用文档：<a
                    href="https://www.murphysec.com/docs/faqs/integration/jetbrains-ide-plugin.html">https://www.murphysec.com/docs/faqs/integration/jetbrains-ide-plugin.html</a></em>
            </td>
        </tr>
        <tr>
            <td><strong>方式3：接入GitLab进行漏洞检测排查</strong><em>使用文档：<a
                    href="https://www.murphysec.com/docs/faqs/integration/gitlab.html">https://www.murphysec.com/docs/faqs/integration/gitlab.html</a></em>
            </td>
        </tr>
        <tr>
            <td><strong>更多排查方式：</strong><em><a
                    href="https://www.murphysec.com/docs/faqs/integration/">https://www.murphysec.com/docs/faqs/integration/</a></em>
            </td>
        </tr>
        </tbody>
    </table>
</figure>
<h1>原文链接</h1>
<p><a href="https://zhi.oscs1024.com/43979.html">https://zhi.oscs1024.com/43979.html</a></p>