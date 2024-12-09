---
title: TranslateResult
description: Learn how to write and customize your documentation.
---


  <div class="text-base leading-7 text-gray-700 dark:text-gray-400">
    <h3 id="fetch-fanyi" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white">获取异步翻译结果</h3>
    <p class="mt-6">
        文本/单个网页翻译可以直接从响应实体中获取翻译结果，对于文档/视频翻译，
        你可以通过翻译任务结果查询接口异步查询文档、视频等业务类型的翻译结果，
        并通过 result_url 字段获取翻译结果的下载链接。
    </p>
    <p class="mt-6 font-semibold">请求参数</p>
    <dl class="divide-y divide-gray-200 overflow-x-auto">
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求URL</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
                https://geekai.co/api/v1/fanyi/:uuid <br>
                <code>:uuid</code> 即提交文档翻译任务成功后返回的 uuid 字段值
            </dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求方式</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">GET</dd>
        </div>
        <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">是否需要认证</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">是</dd>
        </div>
    </dl>
    <p class="mt-6 font-semibold">响应数据</p>
    <div class="inline-block min-w-full align-middle overflow-x-auto">
        <table class="min-w-full divide-y divide-gray-300">
            <thead>
                <tr>
                    <th scope="col" class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-0 dark:text-gray-400">字段</th>
                    <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">说明</th>
                    <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">非空</th>
                </tr>
            </thead>
            <tbody class="divide-y divide-gray-200">
                <!-- 此处可添加响应数据行 -->
            </tbody>
        </table>
    </div>
    <p class="mt-6">示例响应数据：</p>
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/image-20240409000831367.png" alt="示例响应数据">

  </div>
  