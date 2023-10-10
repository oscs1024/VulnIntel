# Nacos 集群Raft反序列化漏洞 (MPS-x09i-fgr6)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>反序列化</td>
            <td><strong>发现时间</strong></td>
            <td>2023-06-06</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-x09i-fgr6">MPS-x09i-fgr6</a></td>
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
            <td>Nacos是一个用于动态服务发现和配置以及服务管理的平台。
攻击者可以在Nacos集群处理某些Jraft请求时利用Hessian进行无限制的反序列化，从而造成远程代码执行。
由于Nacos默认监听7848端口处理Raft协议请求，攻击者可能通过向7848端口发送恶意构造的数据包利用该漏洞。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-x09i-fgr6">https://www.oscs1024.com/hd/MPS-x09i-fgr6</a></em>
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
        <tr><td rowspan="2">com.alibaba.nacos:nacos-consistency [2.0.0, 2.2.3)</td><td>更新</td><td>将组件 com.alibaba.nacos:nacos-consistency 升级到 2.2.3或更高版本</td></tr><tr><td>缓解措施</td><td>禁止 Raft 协议（默认配置7848端口）接收来自Nacos集群外的请求</td></tr><tr><td rowspan="2">com.alibaba.nacos:nacos-consistency [1.4.0, 1.4.6)</td><td>更新</td><td>将组件 com.alibaba.nacos:nacos-consistency 升级到 2.2.3或更高版本</td></tr><tr><td>缓解措施</td><td>禁止 Raft 协议（默认配置7848端口）接收来自Nacos集群外的请求</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-x09i-fgr6">https://www.oscs1024.com/hd/MPS-x09i-fgr6</a></em></td>
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