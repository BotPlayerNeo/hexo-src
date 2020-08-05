---
title: Django相关
date: 2020-08-06 00:35:34
tags:
---

# Django cors headers

加入Django中间件，使响应头添加跨域相关信息。

settings.py

```python
INSTALLED_APPS = [
    'corsheaders',
]

MIDDLEWARE = [
    # 尽量放在顶部，特别是能产生response的中间件之前，如：Django的CommonMiddleware
    'corsheaders.middleware.CorsMiddleware',
    'django.middleware.common.CommonMiddleware',
]

# 允许所有跨域
CORS_ORIGIN_ALLOW_ALL = True
```