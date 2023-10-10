# 腾讯QQ Windows版客户端1-click远程代码执行风险 (MPS-0z86-njh3)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>从非可信控制范围包含功能例程</td>
            <td><strong>发现时间</strong></td>
            <td>2023-08-21</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-0z86-njh3">MPS-0z86-njh3</a></td>
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
            <td>QQ 是一个多平台即时通信软件。
QQ Windows版客户端 9.7.15之前版本中存在逻辑设计缺陷，当消息中包含引用的文件时，直接点击即完成下载和打开操作，缺少相应风险提醒。
攻击者可能利用该特性诱使用户点击运行恶意木马文件，控制用户主机。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-0z86-njh3">https://www.oscs1024.com/hd/MPS-0z86-njh3</a></em>
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
        <tr><td rowspan="2">QQ Windows版 (-∞, 9.7.15)</td><td>更新</td><td>升级QQ Windows版到 9.7.15 或更高版本</td></tr><tr><td>缓解措施</td><td>谨慎点击消息中引用的文件</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-0z86-njh3">https://www.oscs1024.com/hd/MPS-0z86-njh3</a></em></td>
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