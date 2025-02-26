# autohub-benchmark
This project designs common use scenarios for web-based code, model, and dataset hosting platforms, and provides corresponding prompts and ground truth. These resources can be used to evaluate the localization performance of visual language models (VLMs) in specialized scenarios.

## Model Hosting Platform GUI Inference

| Model     | Platform     | Accuracy (%) | Error (%) | Invalid (%) | Completion Rate (%) |
|-----------|--------------|--------------|-----------|-------------|---------------------|
| AriaUI    | Huggingface  | 70.8         | 12.5      | 6.7         | 100.0               |
|           | ModelScope   | 57.6         | 14.2      | 28.2        | 100.0               |
|           | OpenCSG      | 81.0         | 9.5       | 9.5         | 100.0               |
| CogAgent  | Huggingface  | 73.3         | 26.7      | 0.0         | 100.0               |
|           | ModelScope   | 57.9         | 29.1      | 13.0        | 96.3                |
|           | OpenCSG      | 57.1         | 19.0      | 23.8        | 100.0               |
| Qwen3B    | Huggingface  | 8.3          | 15.8      | 19.2        | 41.7                |
|           | ModelScope   | 0.0          | 28.6      | 20.6        | 49.2                |
|           | OpenCSG      | 4.8          | 4.8       | 9.5         | 19.0                |
| Qwen7B    | Huggingface  | 73.3         | 11.7      | 10.8        | 95.8                |
|           | ModelScope   | 55.5         | 30.2      | 8.5         | 95.2                |
|           | OpenCSG      | 71.4         | 14.3      | 14.3        | 100.0               |
| SeeClick  | Huggingface  | 39.2         | 36.7      | 24.2        | 100.0               |
|           | ModelScope   | 52.4         | 29.0      | 18.6        | 100.0               |
|           | OpenCSG      | 52.4         | 14.3      | 33.3        | 100.0               |
| ShowUI    | Huggingface  | 30.0         | 45.0      | 11.7        | 86.7                |
|           | ModelScope   | 43.3         | 26.7      | 14.3        | 88.9                |
|           | OpenCSG      | 23.8         | 52.4      | 9.5         | 85.7                |

Summery:

| Model     | Accuracy (%) | Error (%) | Invalid (%) | Completion Rate (%) |
|-----------|--------------|-----------|-------------|---------------------|
| AriaUI    | 67.7         | 19.3      | 11.4        | 100.0               |
| CogAgent  | 63.3         | 34.8      | 3.0         | 98.7                |
| Qwen3B    | 4.5          | 10.8      | 12.9        | 62.6                |
| Qwen7B    | 66.9         | 18.8      | 10.1        | 100.0               |
| SeeClick  | 45.6         | 26.2      | 26.8        | 97.9                |
| ShowUI    | 32.1         | 42.8      | 11.6        | 85.0                |

## Code Hosting Platform GUI Inference

| Model     | Platform     | Accuracy (%) | Error (%) | Invalid (%) | Completion Rate (%) |
|-----------|--------------|--------------|-----------|-------------|---------------------|
| AriaUI    | GitCode      | 57.1         | 28.5      | 14.3        | 100.0               |
|           | Gitea        | 71.4         | 28.5      | 0.0         | 100.0               |
|           | Gitee        | 57.1         | 28.5      | 14.3        | 100.0               |
|           | Github       | 71.4         | 14.3      | 14.3        | 100.0               |
|           | GitLab       | 71.4         | 14.3      | 14.3        | 100.0               |
| CogAgent  | GitCode      | 71.4         | 28.5      | 0.0         | 100.0               |
|           | Gitea        | 71.4         | 28.5      | 0.0         | 100.0               |
|           | Gitee        | 100.0        | 0.0       | 0.0         | 100.0               |
|           | Github       | 57.1         | 42.8      | 0.0         | 100.0               |
|           | GitLab       | 85.7         | 14.3      | 0.0         | 100.0               |
| Qwen3B    | GitCode      | 14.2         | 28.5      | 42.8        | 85.7                |
|           | Gitea        | 14.2         | 57.1      | 14.2        | 85.7                |
|           | Gitee        | 14.2         | 42.8      | 28.5        | 100.0               |
|           | Github       | 0.0          | 28.5      | 57.1        | 85.7                |
|           | GitLab       | 14.2         | 28.5      | 28.5        | 71.4                |
| Qwen7B    | GitCode      | 71.4         | 0.0       | 28.5        | 100.0               |
|           | Gitea        | 57.1         | 28.5      | 14.2        | 100.0               |
|           | Gitee        | 28.5         | 57.1      | 14.2        | 100.0               |
|           | Github       | 0.0          | 14.2      | 85.7        | 100.0               |
|           | GitLab       | 85.7         | 14.2      | 0.0         | 100.0               |
| SeeClick  | GitCode      | 28.5         | 48.5      | 28.5        | 100.0               |
|           | Gitea        | 28.5         | 28.5      | 48.5        | 100.0               |
|           | Gitee        | 28.5         | 57.1      | 14.2        | 100.0               |
|           | Github       | 14.2         | 57.1      | 28.5        | 100.0               |
|           | GitLab       | 0.0          | 71.4      | 28.5        | 100.0               |
| ShowUI    | GitCode      | 28.5         | 48.5      | 14.2        | 85.7                |
|           | Gitea        | 57.1         | 48.5      | 0.0         | 100.0               |
|           | Gitee        | 57.1         | 28.5      | 0.0         | 85.7                |
|           | Github       | 48.5         | 14.2      | 28.5        | 85.7                |
|           | GitLab       | 48.5         | 14.2      | 14.2        | 71.4                |

Summery:

| Model     | Platform     | Accuracy (%) | Error (%) | Invalid (%) | Completion Rate (%) |
|-----------|--------------|--------------|-----------|-------------|---------------------|
| AriaUI    | 65.7         | 22.8      | 11.4        | 100.0               |
| CogAgent  | 62.9         | 22.8      | 0.0         | 100.0               |
| Qwen3B    | 11.4         | 37.1      | 37.1        | 85.7                |
| Qwen7B    | 48.5         | 22.9      | 28.6        | 100.0               |
| SeeClick  | 20.0         | 51.4      | 28.6        | 100.0               |
| ShowUI    | 45.7         | 28.6      | 11.4        | 85.7                |