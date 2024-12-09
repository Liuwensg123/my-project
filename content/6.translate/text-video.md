---
title: TextVideo
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
    <h3 id="fanyi-file" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white">
        文档/视频翻译
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
                https://geekai.co/api/v1/fanyi/file
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
                form-data（因为包含文件上传）
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
                                biz_type
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                业务类型
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                是
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                支持file、video，对应文档翻译、视频翻译
                            </td>
                            </tr>
                            <tr>
                            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                                source_file
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                待翻译文件（目前仅支持PDF、MP4）
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                是
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                @/E:/文档/待翻译文件.pdf
                            </td>
                            </tr>
                            <tr>
                            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                                target_lang
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                目标语言
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                是
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                english
                            </td>
                            </tr>
                            <tr>
                            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                                model
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                翻译模型
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                否
                            </td>
                            <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                                gpt-4o-mini(默认值)
                            </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </dd>
        </div>
    </dl>
</div>
    <blockquote class="mt-3 text-sm">
        注：目标语言设置参考附录中的
    <a href="#support-langs" class="underline hover:text-gray-500">
        支持语言列表
    </a>
        ，翻译模型设置参考
    <a href="/models" target="_blank" class="underline hover:text-gray-500">
        系统支持模型列表
    </a>
    </blockquote>
    <p class="mt-6 font-semibold">
        响应数据
    <div class="inline-block min-w-full align-middle overflow-x-auto">
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
                非空
            </th>
            </tr>
        </thead>
        <tbody class="divide-y divide-gray-200">
            <tr>
            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                uuid
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
                翻译任务ID
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
                是
            </td>
            </tr>
            <tr>
            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                status
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500">
                翻译任务状态，pending表示待执行
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500">
                是
            </td>
            </tr>
            <tr>
            <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                message
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500">
                翻译任务消息
            </td>
            <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500">
                否
            </td>
            </tr>
        </tbody>
        </table>
    </div>
    </p>
    <p class="mt-6 font-semibold">
        cURL 请求示例（文档翻译）
    </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">
        <code>
            curl --location --request POST 'https://geekai.co/api/v1/fanyi/file' \
            --header 'Authorization: Bearer {API_KEY}' \
            --form 'biz_type="file"' \
            --form 'target_lang="chinese-simplified"' \
            --form 'source_file=@"/E:/文档/待翻译文件.pdf"'
        </code>
    </pre>
    <p class="mt-6 font-semibold"> Postman 请求示例 
        <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240409000442348.png">
    </p>
    <p class="mt-6 font-semibold"> cURL 请求示例（视频翻译） </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">    
        <code>
            curl --location --request POST 'https://geekai.co/api/v1/fanyi/file' \
            --header 'Authorization: Bearer {API_KEY}' \
            --form 'biz_type="video"' \
            --form 'target_lang="chinese-simplified"' \
            --form 'source_file=@"/E:/文档/待翻译视频.mp4"'
        </code>
    </pre>
  <p class="mt-6 font-semibold"> Postman 请求示例 
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240409002353787.png">
  </p>



