# openclaw-memo

##openclaw clawdbot moltbot add modelscope api 添加魔搭社区api

```
 {
    "models": {
      "providers": {
        "modelscope": {
          "baseUrl": "https://api-inference.modelscope.cn/v1",
          "apiKey": "ms-a61db7c2-e8b2-4687-9047-41d91c16cd6d",
          "api": "openai-completions",
          "models": [
            {
              "id": "ZhipuAI/GLM-4.7",
              "name": "GLM-4.7",
              "reasoning": false,
              "input": ["text"],
              "cost": {
                "input": 0,
                "output": 0,
                "cacheRead": 0,
                "cacheWrite": 0
              },
              "contextWindow": 200000,
              "maxTokens": 128000
            }
          ]
        }
      }
    },
    "agents": {
      "defaults": {
        "model": {
          "primary": "modelscope/ZhipuAI/GLM-4.7"
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
        "maxConcurrent": 2,
        "subagents": {
          "maxConcurrent": 3
        }
      }
    }
  }
```
