# NPM 组件包 epic-geo-ip 等恶意获取主机敏感信息 (MPS-2023-8302)
<figure class="wp-block-table">
    <table>
        <tbody>
        <tr>
            <td><strong>漏洞类型</strong></td>
            <td>内嵌恶意代码</td>
            <td><strong>发现时间</strong></td>
            <td>2023-03-17</td>
            <td><strong>漏洞等级</strong></td>
            <td>低危</td>
        </tr>
        <tr>
            <td><strong>MPS编号</strong></td>
            <td><a href="https://www.oscs1024.com/hd/MPS-2023-8302">MPS-2023-8302</a></td>
            <td><strong>CVE编号</strong></td>
            <td>-</td>
            <td><strong>漏洞影响广度</strong></td>
            <td>极小</td>
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
            <td>当用户安装 1.0.1 版本的 epic-geo-ip、epic-dashboard-widgets、epic-community-api 等npm组件包时会向 lupin.monster 域名发送 get 请求，从而泄漏用户主机的 IP 地址。<br><em>参考链接：<a
                    href="https://www.oscs1024.com/hd/MPS-2023-8302">https://www.oscs1024.com/hd/MPS-2023-8302</a></em>
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
        <tr><td rowspan="1">epic-component-library [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-feature-flag [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-dashboard-widgets [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-deployment-tools [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-event-logging [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-database-utils [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-feedback-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-server-tools [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-geo-ip [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-forum-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-http-client [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-payment-gateway [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-notification-service [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-community-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-launcher-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-graphql-resolvers [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-platform-frontend [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-chat-service [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-crypto-utils [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-firebase-integration [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-analytics [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-metrics [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-sdk [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-game-stats [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-gdpr-compliance [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-image-processing [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-leaderboard-service [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-license-validator [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-moderation-tools [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-platform-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-profanity-filter [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-push-notification [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-rate-limiting [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-reporting-tools [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-build-tools [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-dev-portal-backend [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-billing-api [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-cloud-save [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr><tr><td rowspan="1">epic-dev-portal-frontend [1.0.1, 1.0.1]</td><td>替换组件</td><td>避免使用受影响的组件包</td></tr>
        <tr>
            <td colspan="3"><em>参考链接：</em><em><a
                    href="https://www.oscs1024.com/hd/MPS-2023-8302">https://www.oscs1024.com/hd/MPS-2023-8302</a></em></td>
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