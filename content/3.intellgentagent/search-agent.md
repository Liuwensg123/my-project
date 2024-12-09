---
title: SearchAgent
description: Learn how to write and customize your documentation.
---


<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
  <h3 id="fetch-agent" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white">
    查询智能体
  </h3>
  <p class="mt-6">
    智能体创建或更新成功后，可以通过查询接口检查智能体训练状态。
  </p>
  <p class="mt-6 font-semibold">
    请求参数
  </p>
  <dl class="divide-y divide-gray-200 overflow-x-auto">
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
      <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求URL
      </dt>
      <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        https://geekai.co/api/v1/agent/:uuid  
        <code>:uuid</code> 即创建智能体成功后返回的 uuid 字段值
      </dd>
    </div>
    <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
      <dt class="text-sm font-medium leading-6 text-gray-900 dark:text-gray-400">
        请求方式
      </dt>
      <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0 lg:-ml-24 dark:text-gray-400">
        GET
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
  </dl>
  <p class="mt-6 font-semibold">
    响应数据
  </p>
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
          <th scope="col" class="whitespace-nowrap px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">
            非空
          </th>
        </tr>
      </thead>
      <tbody class="divide-y divide-gray-200">
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
            uuid
          </td>
          <td class="whitespace-auto px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            智能体ID
          </td>
          <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            是
          </td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
            name
          </td>
          <td class="whitespace-auto px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            智能体名称
          </td>
          <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            是
          </td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
            logo
          </td>
          <td class="whitespace-auto px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            智能体logo
          </td>
          <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            否
          </td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
            desc
          </td>
          <td class="whitespace-auto px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            智能体描述
          </td>
          <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            是
          </td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">
            status
          </td>
          <td class="whitespace-auto px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            训练状态，running表示训练中，done表示训练完成，failed表示失败
          </td>
          <td class="whitespace-nowrap px-3 py-4 text-sm font-medium text-gray-500 dark:text-gray-400">
            是
          </td>
        </tr>
      </tbody>
    </table>
  </div>
  <p class="mt-6">
    示例响应数据：
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/07/14/4d3c700f4164813a2c5549b86984edb.png">
  </p>


</div>