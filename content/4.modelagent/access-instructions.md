---
title: AcessInstruction
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400" id="docs">
    <h2 id="ai-proxy" class="text-2xl font-bold tracking-tight text-gray-900 dark:text-white"> 模型代理 </h2>
    <p class="mt-6"> 极客智坊提供了与第三方AI服务/工具/客户端集成的接口，通过该接口，你可以轻松通过极客智坊代理
    <a href="/models" target="_blank" class="underline hover:text-gray-500">系统支持的100+模型列表</a>中所有模型的API请求。所有模型请求参数和响应数据格式统一和 OpenAI 对齐以适配绝大部分工具，也就是说支持配置 OpenAI 的工具/客户端都可以使用极客智坊 API 作为平替，且价格更加低廉，其中最常用的 OpenAI 所有模型价格最低仅为官方价的1折。 </p>
    <p class="mt-6"> 对于开发者而言，你当然也可以通过这个AI模型代理服务以更底价格、更简单的上手方式（通过统一接口调用上百种AI模型）构建自己的AI应用,无需再去各个平台注册账号、充值、学习不同平台API调用方式以及后续繁琐的token消耗管理。 </p>
    <p class="mt-6 font-semibold"> 极客智坊底层通过接入不同第三方代理/低价token资源池来保持价格始终处于业界最低水平，并且通过算法在低价和可用性之间自动选择最佳服务链路为您的API调用保驾护航，让更多的开发者和极客用户能够以更低成本享受到AI技术带来的便利。 </p>
    <h3 id="proxy-api" class="mt-6 text-xl font-bold tracking-tight text-gray-900 dark:text-white"> 接入说明 </h3>
    <p class="mt-6 font-semibold "> 请求参数 </p>
    <dl class="divide-y divide-gray-200 overflow-x-auto ">
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-500 dark:text-gray-400">请求URL</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400"> 对话请求URL：https://geekai.co/api/v1/chat/completions<br> 海外加速URL：https://global.geekai.co/api/v1/chat/completions (国外IP调用这个URL速度更快)<br> 智库请求URL：https://geekai.co/api/agent/{智能体ID}/v1/chat/completions </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-500 dark:text-gray-400">请求方式</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">POST </dd>
        </div>
            <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0 dark:text-gray-400">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求数据格式</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">json </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0 ">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">是否需要认证</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">是</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0 dark:text-gray-400">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-500 dark:text-gray-400">请求参数</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24">
                <div class="inline-block min-w-full align-middle">
                    <table class="min-w-full divide-y divide-gray-300 dark:text-gray-500">
                        <thead>
                            <tr>
                                <th scope="col" class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-0 dark:text-gray-400"> 字段</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400"> 说明 </th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400"> 必填 </th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400"> 示例 </th>
                            </tr>
                        </thead>
                        <tbody class="divide-y divide-gray-200">
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">model</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">对话模型</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">否</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500">gpt-4o-mini(默认值)</td>
                            </tr>
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">messages</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">消息列表(智库请求不需要提供system消息)</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">是</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">[{content:"系统提示",role:"system"},{content:"你好",role:"user"},{content:"你好",role:"assistant"},{content:"今天几号",role:"user"}}...]</td>
                            </tr>
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">stream</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">是否返回流式响应，默认false</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">否</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">可设置为true返回流式响应</td>
                            </tr>
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">interneted</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">是否联网</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">否</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">false表示不联网（默认），true表示联网</td>
                            </tr>
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">sess_id</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">会话ID，用于将有关联的多个对话串联起来</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">否</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-400">第三方应用自行实现的会话ID</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </dd>
        </div>
    </dl>
</div>
    <blockquote class="mt-3 text-sm"> 注：对话模型设置参考<a href="/models" target="_blank" class="underline hover:text-gray-500">系统支持模型列表</a>。 OpenAI模型支持图片对话。对于不支持自定义 Claude 请求 URL 的应用，可以通过新增自定义模型<code>geekai-coder</code>进行转发（示例见下面的 <a href="#cursor" class="underline hover:text-gray-500">Cursor配置</a>）。 </blockquote>
    <p class="mt-6"> 响应数据根据是否是流式响应而变化，可以参考下面的请求示例进行判断： </p>
    <p class="mt-6 font-semibold"> cURL 请求示例 </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto"> <code>
            curl --location --request POST 'https://geekai.co/api/v1/chat/completions' \
            --header 'Authorization: Bearer {API_KEY}' \
            --header 'Content-Type: application/json' \
            --data-raw '{
                "model": "gpt-4o-mini",
                "messages": [
                    {
                        "role": "user",
                        "content": "你好"
                    }
                ],
                "stream": false
            }'
        </code>
    </pre>
    <p class="mt-6 font-semibold"> Postman 请求流式响应示例 
        <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/21/image-20240921172301681.png">
    </p>
    <p class="mt-6 font-semibold"> Postman 请求非流式响应示例 <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/21/image-20240921172143432.png"></p>
</div>
