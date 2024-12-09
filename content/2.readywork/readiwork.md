---
title: Readywork
description: Learn how to write and customize your documentation.
---

<div class="text-base leading-7 text-gray-700 dark:text-gray-400 ">
    <h2 id="getting-set-up" class="text-2xl font-bold tracking-tight text-gray-900 dark:text-white"> 准备工作 </h2>
    <p class="mt-6"> 
        第三方应用可以通过调用 API 接口访问极客智坊提供的各类 AI 服务。目前开放了模型代理、AI智能体、极客翻译和万能答题，后续会根据客户需要逐步放开更多服务的 API 接口。
    </p>
    <p class="mt-6"> 调用过程中遇到任何问题，请点击顶部右上角问题反馈图标与极客智坊工程师沟通。 </p>
    <h3 id="access-token" class="mt-6 text-xl font-bold tracking-tight text-gray-900 dark:text-white"> API KEYs </h3>
    <p class="mt-6"> 为了保证 API 调用的安全性，需要在请求头中添加 Authorization 字段，值为 <code>Bearer {API_KEY}</code>，其中 
        <code>{API_KEY}</code> 为你的 API 令牌，可以在令牌管理页面查看和创建： 
    </p>
    <p class="mt-6">
        <a href="/user/api_keys" target="_blank" class="btn rounded-md bg-green-600 px-3 py-2 text-center text-sm font-semibold text-white shadow-sm hover:bg-green-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-green-600"> API 令牌管理 </a>
    </p>
    <p class="mt-6"> 
        API 接口调用计费目前仅支持金币扣费，具体价格信息请参考 
        <a href="/models" target="_blank" class="underline hover:text-gray-500">系统支持模型列表</a>，
        如果调用 API 提示余额不足请通过  <a href="/credit/plans" target="_blank" class="underline hover:text-gray-500">充值金币</a>
        页面充值（你可以在 <a href="/user/balances" target="_blank" class="underline hover:text-gray-500">可用额度</a> 
        页面查看自己的剩余额度）。
    </p>
</div>


