# Laravel框架limit和offset处存在SQL注入 (MPS-19wf-rmek)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>SQL注入</td>
            <td><strong>发现时间</strong></td>
            <td>2024-05-16</td>
            <td><strong>漏洞等级</strong></td>
            <td>严重</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-19wf-rmek">MPS-19wf-rmek</a></td>
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
            <td>Laravel是Laravel社区的一个Web 应用程序框架。 
同时使用SQL Server数据库和Laravel框架，并且Web应用允许用户输入参数直接传递参数到limit和offset函数，存在SQL注入风险。其他数据库如MySQL和Postgres不受此漏洞影响。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-19wf-rmek">https://www.oscs1024.com/hd/MPS-19wf-rmek</a></em>
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
        <tr><td rowspan="1">laravel/framework [6.0.0, 6.20.26)</td><td>缓解措施</td><td>对用户输入的参数进行验证或预处理，确保传至分页函数(如：limit、offset、skip和take)时为整数</td></tr><tr><td rowspan="1">laravel/framework [7.0.0, 7.30.5)</td><td>升级</td><td>将组件 laravel/framework 升级至 7.30.5 及以上版本</td></tr><tr><td rowspan="1">laravel/framework [8.0.0, 8.40.0)</td><td>升级</td><td>将组件 laravel/framework 升级至 8.40.0 及以上版本</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-19wf-rmek">https://www.oscs1024.com/hd/MPS-19wf-rmek</a></em></td>
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
<p><a href="https://zhi.oscs1024.com/42921.html">https://zhi.oscs1024.com/42921.html</a></p>