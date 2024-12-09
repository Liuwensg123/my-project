---
title: TextWebpage
description: Learn how to write and customize your documentation.
---


  <div class="text-base leading-7 text-gray-700 dark:text-gray-400">
    <h2 id="fanyi-ai" class="text-2xl font-bold tracking-tight text-gray-900 dark:text-white"> 极客翻译 </h2>
    <h3 id="fanyi-text" class="mt-6 text-xl font-bold tracking-tight text-gray-900 dark:text-white">
        文本/网页翻译
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
        https://geekai.co/api/v1/fanyi/text
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
                    biz_type
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    业务类型
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    是
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    支持text、link，对应文本翻译、网页翻译
                </td>
                </tr>
                <tr>
                <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
                    source_text
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    待翻译文本（网页翻译则填写网页URL）
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    是
                </td>
                <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">
                    你好，世界！
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
    <p class="mt-6">
        响应数据根据是否是流式响应而变化，可以参考下面的请求示例进行判断：
    </p>
    <p class="mt-6 font-semibold">
        cURL 请求示例（文本翻译）
    </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">
        <code>
            curl --location --request POST 'https://geekai.co/api/v1/fanyi/text'  \
            --header 'Authorization: Bearer {API_KEY}' \
            --header 'Content-Type: application/json' \
            --data-raw '{
                "biz_type": "text",
                "source_text": "你好，世界！",
                "target_lang": "english",
                "stream": true
            }'
        </code>
    </pre>
    <p class="mt-6 font-semibold">
        cURL 请求示例（网页翻译）
    </p>
    <pre class="mt-6 bg-slate-100 flex flex-start items-center justify-start p-4 overflow-x-auto">
        <code>
            curl --location --request POST 'https://geekai.co/api/v1/fanyi/text'  \
            --header 'Authorization: Bearer {API_KEY}' \
            --header 'Content-Type: application/json' \
            --data-raw '{
                "biz_type": "link",
                "source_text": "https://openai.com/about", 
                "target_lang": "chinese-simplified",
                "stream": true
            }'
        </code>
    </pre>

  
 </blockquote>

</div>