# 禅道项目管理系统身份认证绕过风险 (MPS-djcs-koe8)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>身份验证不当</td>
            <td><strong>发现时间</strong></td>
            <td>2024-04-26</td>
            <td><strong>漏洞等级</strong></td>
            <td>高危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-djcs-koe8">MPS-djcs-koe8</a></td>
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
            <td>禅道(ZenTao)项目管理系统是国产开源管理软件，提供整套工具来帮助团队管理整个软件开发生命周期，包括需求管理、迭代计划、任务分配、缺陷跟踪、文档管理和测试用例管理等功能。
受影响版本中由于对 API 鉴权不当，未授权的攻击者可绕过身份校验调用任意API，进而通过修改管理员密码登陆系统，结合经过身份校验的远程代码执行漏洞控制目标服务器。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-djcs-koe8">https://www.oscs1024.com/hd/MPS-djcs-koe8</a></em>
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
        <tr><td rowspan="1">禅道项目管理系统 [16.0, 18.12)</td><td>升级</td><td>将组件 禅道项目管理系统 升级至 18.12 及以上版本</td></tr><tr><td rowspan="1">禅道项目管理系统 [6.0, 8.12)</td><td>升级</td><td>将组件 禅道项目管理系统 升级至 8.12 及以上版本</td></tr><tr><td rowspan="1">禅道项目管理系统 [3.0, 4.12)</td><td>升级</td><td>将组件 禅道项目管理系统 升级至 4.12 及以上版本</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-djcs-koe8">https://www.oscs1024.com/hd/MPS-djcs-koe8</a></em></td>
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
<p><a href="https://zhi.oscs1024.com/42884.html">https://zhi.oscs1024.com/42884.html</a></p>