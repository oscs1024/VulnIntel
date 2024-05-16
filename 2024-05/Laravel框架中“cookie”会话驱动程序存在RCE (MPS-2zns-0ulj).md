# Laravel框架中“cookie”会话驱动程序存在RCE (MPS-2zns-0ulj)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>代码注入</td>
            <td><strong>发现时间</strong></td>
            <td>2024-05-16</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-2zns-0ulj">MPS-2zns-0ulj</a></td>
            <td><strong>CVE编号</strong></td>
            <td>-</td>
            <td><strong>漏洞影响广度</strong></td>
            <td></td>
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
            <td>Laravel是Laravel社区的一个Web 应用程序框架。 
受影响版本中，当应用程序使用“cookie”会话驱动的并且暴露了encryption oracle时会受到远程代码执行的漏洞影响。
encryption oracle是一种机制，其中任意用户输入加密后被显示或暴露给用户。使得用户能够为任何明文字符串生成有效的Laravel签名加密字符串，从而允许他们在应用程序使用“cookie”驱动程序时构造Laravel会话有效负载。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-2zns-0ulj">https://www.oscs1024.com/hd/MPS-2zns-0ulj</a></em>
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
        <tr><td rowspan="1">laravel/framework [4.1.0, 6.18.31)</td><td>升级</td><td>将组件 laravel/framework 升级至 6.18.31 及以上版本</td></tr><tr><td rowspan="1">laravel/framework [7.0.0, 7.22.4)</td><td>升级</td><td>将组件 laravel/framework 升级至 7.22.4 及以上版本</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-2zns-0ulj">https://www.oscs1024.com/hd/MPS-2zns-0ulj</a></em></td>
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
<p><a href="https://zhi.oscs1024.com/42917.html">https://zhi.oscs1024.com/42917.html</a></p>