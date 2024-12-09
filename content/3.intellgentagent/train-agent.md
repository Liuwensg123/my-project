---
title: TrainAgent
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
    <h3 id="embed-agent" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white">训练智能体</h3>
    <p class="mt-6">你可以通过智能体训练接口向指定智能体添加训练文件（支持批量上传）进行智能体训练。</p>
    <p class="mt-6 font-semibold">请求参数</p>
    <dl class="divide-y divide-gray-200 overflow-x-auto">
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求URL</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
                https://geekai.co/api/v1/agent/:uuid/embed <br>
                <code>:uuid</code> 即创建智能体成功后返回的 uuid 字段值
            </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求方式</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">PATCH</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求数据格式</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">form-data（因为包含文件上传）</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">是否需要认证</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">是</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求参数</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24">
                <div class="inline-block min-w-full align-middle">
                    <table class="min-w-full divide-y divide-gray-300">
                        <thead>
                            <tr>
                                <th scope="col" class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-0 dark:text-gray-400">字段</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">说明</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">必填</th>
                                <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">示例</th>
                            </tr>
                        </thead>
                        <tbody class="divide-y divide-gray-200">
                            <tr>
                                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">embed_files</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">本地训练文件路径（支持批量上传）</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">是</td>
                                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">/E:/文档/待训练文件.pdf</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </dd>
        </div>
    </dl>
    <p class="mt-6">响应数据和创建智能体一样，略。</p>
    <p class="mt-6 font-semibold">cURL 请求示例</p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">
        <code>
            curl --location --request PATCH 'https://geekai.co/api/v1/agent/be9062c1-68d5-48ee-b74e-fab6d864bc29/embed' \
            --header 'Authorization: Bearer {API_KEY}' \
            --form 'embed_files=@"/E:/文档/极客智坊/训练文件1.txt"' \
            --form 'embed_files=@"/E:/文档/极客智坊/训练文件2.txt"' \
            --form 'embed_files=@"/E:/文档/极客智坊/训练文件3.txt"'
        </code>
    </pre>
    <p class="mt-6 font-semibold">Postman 请求示例</p>
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240420020516665.png">
</div>