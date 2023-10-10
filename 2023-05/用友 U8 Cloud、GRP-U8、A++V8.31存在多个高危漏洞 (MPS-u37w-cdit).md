# 用友 U8 Cloud、GRP-U8、A++V8.31存在多个高危漏洞 (MPS-u37w-cdit)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>注入</td>
            <td><strong>发现时间</strong></td>
            <td>2023-05-17</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-u37w-cdit">MPS-u37w-cdit</a></td>
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
            <td>用友 U8 Cloud、GRP-U8 是用友软件公司开发的提供企业资源管理解决方案的产品。 
用友 U8 Cloud 存在3个高危漏洞，分别为LoggingConfigServlet反序列化漏洞、BeanShell远程代码执行漏洞、commons-beanutils 远程代码执行漏洞。
用友 GRP-U8 存在3个高危漏洞，分别为forgetPassword_old.jsp SQL注入漏洞、XML实体注入漏洞、XXNode SQL注入漏洞。
用友 A++V8.31 存在1个高危漏洞，为selectGlaDatasourcePreview接口SQL注入漏洞。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-u37w-cdit">https://www.oscs1024.com/hd/MPS-u37w-cdit</a></em>
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
        <tr><td rowspan="1">用友 [U8cloud, U8cloud]</td><td>补丁</td><td>官方已发布补丁：https://security.yonyou.com/#/patchList</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-u37w-cdit">https://www.oscs1024.com/hd/MPS-u37w-cdit</a></em></td>
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