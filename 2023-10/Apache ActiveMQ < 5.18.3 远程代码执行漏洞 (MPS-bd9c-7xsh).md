# Apache ActiveMQ < 5.18.3 远程代码执行漏洞 (MPS-bd9c-7xsh)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>反序列化</td>
            <td><strong>发现时间</strong></td>
            <td>2023-10-25</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-bd9c-7xsh">MPS-bd9c-7xsh</a></td>
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
            <td>Apache ActiveMQ 是美国阿帕奇（Apache）基金会的一套开源的消息中间件，它支持Java消息服务、集群、Spring Framework等。
ActiveMQ默认开放了61616端口用于接收OpenWire协议消息，由于针对异常消息的处理存在反射调用逻辑，攻击者可能通过构造恶意的序列化消息数据加载恶意类，执行任意代码。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-bd9c-7xsh">https://www.oscs1024.com/hd/MPS-bd9c-7xsh</a></em>
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
        <tr><td rowspan="1">org.apache.activemq:activemq-openwire-legacy [5.18.0, 5.18.3)</td><td>升级</td><td>将组件 org.apache.activemq:activemq-openwire-legacy 升级至 5.18.3 及以上版本</td></tr><tr><td rowspan="1">org.apache.activemq:activemq-client (-∞, 5.17.6)</td><td>升级</td><td>将组件 org.apache.activemq:activemq-client 升级至 5.17.6 及以上版本</td></tr><tr><td rowspan="1">org.apache.activemq:activemq-openwire-legacy (-∞, 5.17.6)</td><td>升级</td><td>将组件 org.apache.activemq:activemq-openwire-legacy 升级至 5.17.6 及以上版本</td></tr><tr><td rowspan="1">org.apache.activemq:activemq-client [5.18.0, 5.18.3)</td><td>更新</td><td>升级至5.15.16, 6.0.0, 5.18.3, 5.17.6, 5.16.7或更高版本</td></tr><tr><td rowspan="1">activemq [5.18.0, 5.18.3)</td><td>升级</td><td>将组件 activemq 升级至 5.18.3 及以上版本</td></tr><tr><td rowspan="1">activemq (-∞, 5.17.6)</td><td>升级</td><td>将组件 activemq 升级至 5.17.6 及以上版本</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-bd9c-7xsh">https://www.oscs1024.com/hd/MPS-bd9c-7xsh</a></em></td>
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
<p><a href="https://zhi.oscs1024.com/16135.html">https://zhi.oscs1024.com/16135.html</a></p>