---
title: Pricing-desciption
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
  <h3 id="model-prices" class="mt-6 text-xl font-bold tracking-tight text-gray-900 dark:text-white">模型价格分级说明</h3>
  <p class="mt-6">
    极客智坊基于官方价格对系统支持的所有AI模型做了分级，以方便开发者归类和选择：
  </p>
  <div class="overflow-x-auto">
    <table class="min-w-full divide-y divide-gray-300">
      <thead>
        <tr>
          <th scope="col" class="py-3.5 pl-4 pr-3 text-left text-sm font-semibold text-gray-900 sm:pl-0 dark:text-gray-400">模型级别</th>
          <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">价格区间</th>
          <th scope="col" class="px-3 py-3.5 text-left text-sm font-semibold text-gray-900 dark:text-gray-400">代表模型</th>
        </tr>
      </thead>
      <tbody class="divide-y divide-gray-200">
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">免费模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">所有场景免费使用</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">gpt-4o-mini、glm-4-flash</td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">B级模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">API输入价格在10元/百万tokens以内，个人版会员可站内免费使用</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">claude-3-5-haiku-latest、doubao-pro-128k</td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">A级模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">API输入价格在10-40元/百万tokens区间，专业版会员可站内免费使用</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">gpt-4o、claude-3-5-sonnet-latest</td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0">S级模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">一般各AI平台顶级旗舰模型，输入价格在40-120元之间</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">o1-preview、ernie-4.0-8k</td>
        </tr>
        <tr>
          <td class="whitespace-nowrap py-4 pl-4 pr-3 text-sm font-medium text-gray-900 sm:pl-0 dark:text-gray-400">S+级模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">价格超过120元的AI模型</td>
          <td class="whitespace-nowrap px-3 py-4 text-sm text-gray-500 dark:text-gray-400">gpt-4</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

  <blockquote class="mt-3 text-sm text-gray-500 dark:text-gray-400">
    声明：以上分级仅以价格维度划分，不代表模型质量、性能等其他维度的评价。
  </blockquote>

  <p class="mt-6">
    与此同时，极客智坊AI模型代理服务底层引擎支持在运行时动态选择最佳API代理进行对话，以最大化降低API调用成本，这个最佳包含两个层面 —— 一个是价格，一个是可用性，价格低不可用不是最佳，可用但价格高也不是最佳，最佳意味着低价与可用性的动态平衡。
  </p>

  <p class="mt-6">
    这对于使用极客智坊AI模型代理API构建AI应用的开发者来说是一大利好，也是极客智坊对构建<b class="text-green-600">多快好省AI模型评测与代理平台</b>愿景的体现。这里有必要解释一下这个<b>多快好省</b>的具体含义：
  </p>
  
  <ul class="mt-6 list-disc pl-6">
    <li><b>多</b>：极客智坊引入了对主流AI平台上百种AI模型的支持，并且这一数量还在继续增加，接下来还会陆续引入对文生图、文生音频、文生视频模型的支持，使得开发者可以在一个平台调用上百种AI模型；</li>
    <li><b>快</b>：极客智坊通过网络、账号、服务器、数据库、缓存、队列、代码优化等多个层面立体式提升AI模型代理服务的并发与访问速度，让开发者没有AI技术中间件性能层面的后顾之忧；</li>
    <li><b>好</b>：极客智坊将以匠心态度持续为极客&开发者以更低成本访问AI模型、构建AI应用提供专业优质的工具与平台服务，让大家用的省心、用的放心；</li>
    <li><b>省</b>：省有两个层面 —— 一个是技术学习与运维成本：开发者可以在极客智坊平台以同一格式同一账号轻松访问上百种AI模型，极大省去了不同AI平台注册账号、充值续费、API开发的学习与维护成本；另一个是实打实的API调用成本：极客智坊模型代理底层引擎支持通过算法在多个维度（优先级、渠道、价格、可用性）实时动态选择最佳API代理提供AI底层服务，切实降低开发者调用AI模型API的财务成本，目前已经支持OpenAI、Claude、Gemini、智谱清言等多个平台的低价API代理服务，你可以在极客智坊<a href="/models" target="_blank" class="underline hover:text-gray-500">模型广场</a>查看所有AI模型及其价格。这样一来，开发者就可以放心大胆通过极客智坊模型代理服务低成本/零成本构建AI应用。
    </li>
  </ul>
</div>
