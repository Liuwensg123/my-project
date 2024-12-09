---
title: Cursor
description: Learn how to write and customize your documentation.
---


<div class="text-base leading-7 text-gray-700 dark:text-gray-400">
  <h3 id="cursor" class="text-xl font-bold tracking-tight text-gray-900 dark:text-white"> Cursor </h3>
  <p class="mt-6"> 打开 
    <a target="_blank" class="underline hover:text-gray-500" href="https://www.cursor.com/">Cursor</a> 
    配置界面，填入极客智坊 API 接口 URL 和 API_KEY： 
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/22/image-20240922111526463.png">
  </p>
  <blockquote class="mt-3 text-sm"> 注意：接口 URL 后面要带 <code>/v1</code> 后缀。 </blockquote>
  <p class="mt-3"> 配置完成后，点击 Verify 进行验证，验证通过后保存设置，然后进入对话界面即可通过极客智坊代理 OpenAI 模型进行对话： 
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/22/image-20240922112948509.png">
  </p>
  <p class="mt-3"> 如果你觉得其他模型编写代码质量更高，比如 Claude-3.5-Sonnet，但 Cursor 不支持自定义 Claude 请求 URL，这可以通过自定义模型<code>geekai-coder</code>进行转发来达到曲线救国的效果： 
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/22/image-20240922223931936.png">
  </p>
  <p class="mt-3"> 极客智坊在接收到该模型请求时，会自动转发到 Claude-3.5-Sonnet 官方接口，所以你可以在 Cursor 中直接使用： 
    <img class="mt-2" src="https://cdn.geekai.co/storage/2024/09/22/image-20240922224117109.png">
  </p>
</div>
