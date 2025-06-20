# 泛微e-cology < v10.75 /js/hrm/getdata.jsp 未授权SQL注入漏洞 (MPS-ui2a-byv3)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>SQL注入</td>
            <td><strong>发现时间</strong></td>
            <td>2025-06-17</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-ui2a-byv3">MPS-ui2a-byv3</a></td>
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
            <td>泛微e-cology是泛微公司开发的协同管理应用平台。
受影响版本中，/js/hrm/getdata.jsp 存在 SQL 注入漏洞，由于其中调用 weaver.hrm.common.AjaxManager.getData 方法，用户可控参数经过两次 URL 解码后，最终被拼接至：append(" and t.id = ").append(StringUtil.vString(map.get("id")))处，导致 SQL 注入漏洞，攻击者可能进一步写入Webshell导致远程代码执行。
修复版本通过对用户可控的参数进行强制数字转换，防止SQL注入漏洞。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-ui2a-byv3">https://www.oscs1024.com/hd/MPS-ui2a-byv3</a></em>
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
        <tr><td rowspan="1">e-cology (-∞, 10.75)</td><td>升级</td><td>将组件 e-cology 升级至 10.75 及以上版本</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-ui2a-byv3">https://www.oscs1024.com/hd/MPS-ui2a-byv3</a></em></td>
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
<p><a href="https://zhi.oscs1024.com/43077.html">https://zhi.oscs1024.com/43077.html</a></p>