# 泛微 e-cology <10.58.3 任意文件上传漏洞 (MPS-rkja-iwgs)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>任意文件上传</td>
            <td><strong>发现时间</strong></td>
            <td>2023-07-26</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-rkja-iwgs">MPS-rkja-iwgs</a></td>
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
            <td>泛微协同管理应用平台(e-cology)是一套企业大型协同管理平台。
泛微 e-cology 10.58.3之前版本存在任意文件上传漏洞，由于上传接口身份认证缺失，未经过身份验证的攻击者可以构造恶意请求将文件上传至服务器，攻击者可能通过上传jsp文件，从而远程执行任意命令。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-rkja-iwgs">https://www.oscs1024.com/hd/MPS-rkja-iwgs</a></em>
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
        <tr><td rowspan="1">e-cology9 (-∞, 10.58.3)</td><td>更新</td><td>升级e-cology9到 10.58.3 或更高版本</td></tr><tr><td rowspan="2">e-cology8 (-∞, 10.58.3)</td><td>更新</td><td>升级e-cology8到 10.58.3 或更高版本</td></tr><tr><td>补丁</td><td>官方已发布补丁：https://www.weaver.com.cn/cs/securityDownload.asp#</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-rkja-iwgs">https://www.oscs1024.com/hd/MPS-rkja-iwgs</a></em></td>
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