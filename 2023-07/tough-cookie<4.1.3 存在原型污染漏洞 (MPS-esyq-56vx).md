# tough-cookie<4.1.3 存在原型污染漏洞 (MPS-esyq-56vx)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>原型污染</td>
            <td><strong>发现时间</strong></td>
            <td>2023-07-01</td>
            <td><strong>漏洞等级</strong></td>
            <td>中危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-esyq-56vx">MPS-esyq-56vx</a></td>
            <td><strong>CVE编号</strong></td>
            <td>-</td>
            <td><strong>漏洞影响广度</strong></td>
            <td>一般</td>
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
            <td>tough-cookie 是一个用于处理 HTTP cookie 的 JavaScript 库。
受影响版本中的 rejectPublicSuffixes=false 模式下使用 CookieJar 存在原型污染漏洞，攻击者可修改 Domain=__proto__; 原型属性执行恶意代码。
用户可通过在 Map 中存储 cookie 或使用 this.idx = Object.create(null) 创建 idx 变量缓解此漏洞。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-esyq-56vx">https://www.oscs1024.com/hd/MPS-esyq-56vx</a></em>
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
        <tr><td rowspan="2">tough-cookie [2.3.0, 4.1.3)</td><td>更新</td><td>升级tough-cookie到 4.1.3 或更高版本</td></tr><tr><td>缓解措施</td><td>用户可通过在 Map 中存储 cookie 或使用 this.idx = Object.create(null) 创建 idx 变量缓解此漏洞</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-esyq-56vx">https://www.oscs1024.com/hd/MPS-esyq-56vx</a></em></td>
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