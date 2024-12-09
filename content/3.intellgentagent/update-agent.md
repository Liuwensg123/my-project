---
title: UpdateAgent
description: Learn how to write and customize your documentation.
---



<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
  <h3 id="update-agent" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white"> 更新智能体 </h3>
  <p class="mt-6"> 你可以通过更新接口更新一个已存在的智能体。 </p>
  <p class="mt-6 font-semibold"> 请求参数 </p>
  <dl class="divide-y divide-gray-200 overflow-x-auto">
      <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求URL</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
              https://geekai.co/api/v1/agent/:uuid/update <br>
              <code>:uuid</code> 即创建智能体成功后返回的 uuid 字段值
          </dd>
      </div>
      <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求方式</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">PUT</dd>
      </div>
      <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
          <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">请求数据格式</dt>
          <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">form-data</dd>
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
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">name</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">智能体名称</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">是</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">测试智能体</td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">logo</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">智能体Logo图片链接</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">否</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400"></td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">desc</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">智能体描述</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">是</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">测试智能体</td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">model</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">训练模型</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">否</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">deepseek-chat(默认值)</td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">chat_level</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">模型温度</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">否</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">0/1/2/3/4，默认值2，温度越高创造性越高，反之准确性越高</td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">interneted</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">是否联网</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">否</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">0表示不联网（默认），1表示联网</td>
                          </tr>
                          <tr>
                              <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">stream</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">是否流式对话</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">否</td>
                              <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">0表示否，1表示是（默认）</td>
                          </tr>
                      </tbody>
                  </table>
              </div>
          </dd>
      </div>
  </dl>
  <blockquote class="mt-3 text-sm"> 
      注：训练模型设置参考<a href="/models" target="_blank" class="underline hover:text-gray-500">系统支持模型列表</a>。 
  </blockquote>
  <p class="mt-6"> 响应数据和创建智能体一样，略。 </p>
  <p class="mt-6"> 请求示例也和创建智能体差不多，略。 </p>

</div>