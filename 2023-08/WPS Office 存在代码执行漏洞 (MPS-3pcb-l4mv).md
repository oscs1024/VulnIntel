# WPS Office 存在代码执行漏洞 (MPS-3pcb-l4mv)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>代码注入</td>
            <td><strong>发现时间</strong></td>
            <td>2023-08-09</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-3pcb-l4mv">MPS-3pcb-l4mv</a></td>
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
            <td>WPS Office软件是由金山办公软件股份有限公司自主研发的一款办公软件套装。
受影响版本中，WPS Office 中嵌入的浏览器域名白名单机制存在设计缺陷，攻击者可以利用此漏洞创建恶意文件。
受害者打开文件并点击带有超链接的图片或对象后，可能将远程服务器上的恶意代码下载到指定目录下并执行。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-3pcb-l4mv">https://www.oscs1024.com/hd/MPS-3pcb-l4mv</a></em>
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
        <tr><td rowspan="2">WPS Office 个人版 (-∞, 12.1.0.15324)</td><td>更新</td><td>将WPS Office 个人版升级到 12.1.0.15324 及以上版本</td></tr><tr><td>缓解措施</td><td>避免点击带有超链接的图片或对象</td></tr><tr><td rowspan="2">WPS Office 机构版 (-∞, 11.8.2.12085)</td><td>更新</td><td>将 WPS Office 机构版更新到 11.8.2.12085 或更高版本</td></tr><tr><td>缓解措施</td><td>避免点击带有超链接的图片或对象</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-3pcb-l4mv">https://www.oscs1024.com/hd/MPS-3pcb-l4mv</a></em></td>
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