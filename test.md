```markdown
# Vue 简单主页示例

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>Vue 简单主页</title>
    <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
    <style>
        body { font-family: Arial, sans-serif; margin: 40px; }
        h1 { color: #42b983; }
        button { padding: 8px 16px; margin-top: 10px; }
    </style>
</head>
<body>
    <div id="app">
        <h1>{{ title }}</h1>
        <p>欢迎来到 Vue 主页！</p>
        <button @click="count++">点击次数：{{ count }}</button>
    </div>
    <script>
        const { createApp } = Vue;
        createApp({
            data() {
                return {
                    title: '我的 Vue 主页',
                    count: 0
                }
            }
        }).mount('#app');
    </script>
</body>
</html>
```
```