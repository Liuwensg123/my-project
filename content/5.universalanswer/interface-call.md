---
title: InterfaceCall
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
    <h2 id="dati-ai" class="text-2xl font-bold tracking-tight text-gray-900 dark:text-white"> 万能答题 </h2>
    <h3 id="dati-api" class="mt-6 text-xl font-bold tracking-tight text-gray-900 dark:text-white">
    接口调用
    </h3>
    <p class="mt-6 font-semibold">
    请求参数
    </p>
    <dl class="divide-y divide-gray-200 overflow-x-auto">
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
        <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求URL
        </dt>
        <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        https://geekai.co/api/v1/chat/dati
        </dd>
    </div>
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
        <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求方式
        </dt>
        <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        POST
        </dd>
    </div>
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
        <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求数据格式
        </dt>
        <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        json
        </dd>
    </div>
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
        <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        是否需要认证
        </dt>
        <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        是
        </dd>
    </div>
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
        <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求参数
        </dt>
        <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24">
        <div class="inline-block min-w-full align-middle">
            <table class="min-w-full divide-y divide-gray-300">
            <thead>
                <tr>
                <th scope="col" class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-0 dark:text-gray-400">
                    字段
                </th>
                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">
                    说明
                </th>
                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">
                    必填
                </th>
                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">
                    示例
                </th>
                </tr>
            </thead>
            <tbody class="divide-y divide-gray-200">
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    system
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    系统提示
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    扮演一个文案专家
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    prompt
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    问题
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    是
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    编写一段介绍ChatGPT的广告文案
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    messages
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    历史消息列表
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    [{text:"问题",role:"human"},{text:"回答",role:"ai"}...]
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    model
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    对话模型
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    deepseek-chat(默认值)
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    stream
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    是否返回流式响应，默认false
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    可设置为true返回流式响应
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    interneted
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    是否联网
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    false表示不联网（默认），true表示联网
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    sess_id
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    会话ID，用于将有关联的多个对话串联起来
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    否
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    第三方应用自行实现的会话ID
                </td>
                </tr>
            </tbody>
            </table>
        </div>
        </dd>
    </div>
    </dl>
    <blockquote class="mt-3 text-sm">
    注：对话模型设置参考
    <a href="/models" target="_blank" class="underline hover:text-gray-500">
        系统支持模型列表
    </a>
    </blockquote>
    <p class="mt-6">
    响应数据根据是否是流式响应而变化，可以参考下面的请求示例进行判断：
    </p>
    <p class="mt-6 font-semibold">
    cURL 请求示例
    </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">
    <code>
        curl --location --request POST 'https://geekai.co/api/v1/chat/dati'  \
        --header 'Authorization: Bearer {API_KEY}' \
        --header 'Content-Type: application/json' \
        --data-raw '{
            "prompt": "编写一段介绍ChatGPT的广告文案",
            "stream": false
    </code>
    </pre>
    <p class="mt-6 font-semibold"> Postman 请求流式响应示例 
        <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240414001138207.png">
    </p>
    <p class="mt-6 font-semibold"> Postman 请求非流式响应示例 
        <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240414001233000.png">
    </p>

</div>



