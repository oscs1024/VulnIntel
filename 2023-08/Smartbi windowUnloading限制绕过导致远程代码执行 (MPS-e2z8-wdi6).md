# Smartbi windowUnloading限制绕过导致远程代码执行 (MPS-e2z8-wdi6)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>授权机制不恰当</td>
            <td><strong>发现时间</strong></td>
            <td>2023-08-22</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-e2z8-wdi6">MPS-e2z8-wdi6</a></td>
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
            <td>Smartbi 是思迈特软件旗下的一款商业智能应用，提供了数据集成、分析、可视化等功能，帮助用户理解和使用数据进行决策。
Smartbi V6及其以上版本的 /smartbi/vision/RMIServlet API存在验证不当问题，攻击者可向该接口发送恶意构造的POST请求，并将 url 编码后的恶意 className 和 methodName 参数传入 windowUnloading 参数中绕过权限验证，调用后端接口。
官方在7月3日发布的补丁中，通过校验了post请求参数与URL中参数的一致性进行修复，应用仍可接收content-type为multipart/form-data的请求参数，导致补丁绕过，从而获取系统用户凭据、执行远程代码。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-e2z8-wdi6">https://www.oscs1024.com/hd/MPS-e2z8-wdi6</a></em>
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
        <tr><td rowspan="1">Smartbi [V6, V9]</td><td>补丁</td><td>官方已发布补丁：https://www.smartbi.com.cn/patchinfo</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-e2z8-wdi6">https://www.oscs1024.com/hd/MPS-e2z8-wdi6</a></em></td>
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