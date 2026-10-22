# 学习通全自动学习

基于 `学习通 AI 助手 1.23` 修改的 Tampermonkey 用户脚本，用于学习通课程页的视频播放、翻节、答题与提交串联托管。

> 非官方项目，与超星/学习通无隶属关系。自动化操作可能违反课程或学校规定，请自行评估风险。

## 安装

1. 安装 Tampermonkey（Chrome / Edge）。
2. 打开 [Releases](https://github.com/L-ty-34/cx-auto-study/releases/latest)，下载 `cx-auto-study.user.js` 并安装。
3. 只保留这一个版本，禁用旧版脚本。
4. 打开学习通课程学习页，点击助手面板，在“设置”里配置模型接口和 API Key。

也可以直接打开：

```text
https://raw.githubusercontent.com/L-ty-34/cx-auto-study/main/cx-auto-study.user.js
```

## 主要功能

- 视频播放结束后自动点击“下一节”
- 新页面加载后自动点击视频开始播放
- 答题页点击“一键生成答案”，等待填写完成
- 自动点击“提交”，并等待慢速确认弹窗（约 22 秒）
- 确认后继续下一节，形成顺序托管
- 托管期间“视频不暂停”选项：鼠标移出视频/窗口也继续播放
- 左侧任务栏只保留“题目”“自动点击”“设置”

## 使用与配置

详细步骤见 [使用说明.md](使用说明.md)。

- AI 答题需要配置模型服务；脚本不内置任何 API Key。
- 支持云端 OpenAI 兼容接口，也支持本地 Ollama / LM Studio。
- 顶部 GitHub 按钮指向作者个人主页。

## 更新

脚本已配置：

```js
// @updateURL    https://raw.githubusercontent.com/L-ty-34/cx-auto-study/main/cx-auto-study.user.js
// @downloadURL  https://raw.githubusercontent.com/L-ty-34/cx-auto-study/main/cx-auto-study.user.js
```

发布后 Tampermonkey 会自动检查更新。首次发布前该地址会 404，属于正常现象。

## 来源与许可

- 原始脚本：`学习通 AI 助手 1.23`（作者 Hailin，MIT）
- 本修改版：学习通全自动学习 1.1（修改：L-ty-34）
- 许可证：[MIT](LICENSE)，第三方来源见 [NOTICE](NOTICE)