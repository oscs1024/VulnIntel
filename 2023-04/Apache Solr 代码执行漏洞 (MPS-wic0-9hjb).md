# Apache Solr 代码执行漏洞 (MPS-wic0-9hjb)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>关键资源权限分配不当</td>
            <td><strong>发现时间</strong></td>
            <td>2023-04-15</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-wic0-9hjb">MPS-wic0-9hjb</a></td>
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
            <td>Apache Solr 是一款开源的搜索引擎。
在Apache Solr 受影响版本中，由于Solr默认配置下存在服务端请求伪造漏洞，且SolrResourceLoader中实现了java SPI机制。当Solr以SolrCloud模式启动时，攻击者可以通过构造恶意的solrconfig.xml文件，组合利用从而执行任意java代码。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-wic0-9hjb">https://www.oscs1024.com/hd/MPS-wic0-9hjb</a></em>
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
        <tr><td rowspan="2">org.apache.solr:solr-core [8.10.0, 9.2.0)</td><td>更新</td><td>升级org.apache.solr:solr-core到 9.2.0 或更高版本</td></tr><tr><td>缓解措施</td><td>以 solrcloud 方式部署的机器不出网或添加Solr身份校验。
</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-wic0-9hjb">https://www.oscs1024.com/hd/MPS-wic0-9hjb</a></em></td>
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