# WPS Office 远程代码执行漏洞(WPSSRC-2023-0701绕过) (MPS-qjky-hw9x)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>代码注入</td>
            <td><strong>发现时间</strong></td>
            <td>2023-08-22</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-qjky-hw9x">MPS-qjky-hw9x</a></td>
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
            <td>WPS Office 软件是由金山办公软件股份有限公司自主研发的一款办公软件套装。
由于对 WPSSRC-2023-0701 的修复不充分，WPS Office Windows 版本仍受到远程代码执行的影响。攻击者通过诱导用户打开构造恶意的文档，无需其它操作即可远程执行任意代码，进而完全控制用户主机。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-qjky-hw9x">https://www.oscs1024.com/hd/MPS-qjky-hw9x</a></em>
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
        <tr><td rowspan="1">WPS Office Windows个人版 (-∞, 12.1.0.15355]</td><td>缓解措施</td><td>避免使用 WPS 打开不受信任的文档</td></tr><tr><td rowspan="1">WPS Office Windows机构版 (-∞, 11.8.2.12089]</td><td>缓解措施</td><td>避免使用 WPS 打开不受信任的文档</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-qjky-hw9x">https://www.oscs1024.com/hd/MPS-qjky-hw9x</a></em></td>
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