# openclaw-memo

##openclaw clawdbot moltbot add modelscope api 添加魔搭社区api

```
  "models": {
    "providers": {
      "modelscope": {
        "baseUrl": "https://api-inference.modelscope.cn/v1",
        "apiKey": "XXXXXXXXXX",
        "api": "openai-completions",
        "models": [
          {
            "id": "ZhipuAI/GLM-4.7",
            "name": "ZhipuAI/GLM-4.7",
            "reasoning": false,
            "input": [
              "text"
            ],
            "cost": {
              "input": 0,
              "output": 0,
              "cacheRead": 0,
              "cacheWrite": 0
            },
            "contextWindow": 128000,
            "maxTokens": 8192
          }
        ]
      }
    }
  },
  "agents": {
    "defaults": {
      "model": {
        "primary": "GLM-4.7"
      },
      "models": {
        "modelscope/ZhipuAI/GLM-4.7": {
          "alias": "GLM-4.7"
        }
      },
      "workspace": "/home/neo/.openclaw/workspace",
      "compaction": {
        "mode": "safeguard"
      },
      "maxConcurrent": 4,
      "subagents": {
        "maxConcurrent": 8
      }
    }
  },
```
