---
layout: default
title: Support · 支持
permalink: /support/
lang: en
description: How to get help with Alicia Recorder, and answers to common questions.
---

[English](#english) · [中文](#chinese)
{: .jump}

# Support {#english}

## Getting help

Open an issue on GitHub:
[github.com/Aliciahan/pubweb-aliciarecorderdesktop/issues](https://github.com/Aliciahan/pubweb-aliciarecorderdesktop/issues).
You need a GitHub account to write there.

**Issues are public: anyone can read what you write.** Do not post personal data, recordings, transcripts, notes,
calendar entries or API keys. Describe what you did and what happened, and give the app's version (Settings › About)
and your macOS version.
{: .note}

## Common questions

### Where are my recordings and notes stored?

In the library folder you chose when you set up the app, for example a folder in iCloud Drive: the audio files,
transcripts, summaries and minutes (`.note.md` files), journals and weekly reviews (the `_journal` folder), and the
app's own files about them in a hidden `.alicia` folder. They are ordinary files: you can open them in Finder and back
them up like any other folder.

The app's own data — the search index, settings, downloaded optional models and caches — stays on your Mac: for the
Mac App Store version inside its container in `~/Library/Containers`, for the direct download in
`~/Library/Application Support/AliciaRecorder`. API keys are kept in the macOS keychain. The index can always be
rebuilt from your library folder with Settings › Library › Rebuild Index….

### What is sent to AI providers, and how do I stop it?

Transcription, speaker separation and search run on your Mac and send nothing. Summaries, minutes, journals, weekly
reviews and answers are written by the language model you set up, and the app sends it **text, never audio**: the
transcript and the other items listed in section 4.1 of the [privacy policy]({{ '/privacy/' | relative_url }}).
Before anything goes to a provider outside your Mac and local network, the app asks for your consent and shows what
each task sends.

To stop or limit it:

- **Withdraw your consent** for a provider in Settings › AI Models (“Withdraw Consent”), or delete the provider there,
  which also deletes its API key.
- **Mark a recording “Local Only”** (the checkbox next to its date, or the item in the list's context menu): it then
  only goes to a model on your Mac, your local network or a server you set to be treated as local.
- **Use only a local model**, such as Ollama or LM Studio on your Mac: then nothing leaves your Mac or your network.

Text already sent cannot be called back; ask the provider to delete it. If notes have only a cloud model, a medical
conversation can be sent before the app recognizes it as medical; the privacy policy explains how to avoid that.

### How do the trial and the purchase work?

This is about the Mac App Store version. The app is a free download. In the app you can start a free
**15-day Trial**, an In-App Purchase that costs nothing; after it, a one-time **Full Version** purchase unlocks the
app. It is not a subscription. The price is shown in the app and comes from the App Store for your country or region.

- The trial runs for 15 days from the moment you take it. It belongs to your Apple Account, so reinstalling the app
  or using another Mac does not start it again.
- Without the trial or the Full Version you can still open your library, read, search, play, export and delete your
  recordings and notes, change settings and rebuild the index. New recordings, importing, transcription, writing
  summaries and journals, and questions need the trial or the Full Version.
- A recording that is under way when the trial ends is finished and saved; its processing continues after a
  purchase.
- On another Mac or after reinstalling, use **Restore Purchases** in the app.

Apple handles the trial and the purchase; the app only asks the App Store, on your Mac, whether your Apple Account has
them. The direct download has no trial and no purchase.

### How do I get a refund?

Purchases in the Mac App Store are made with Apple, and only Apple can refund them. Go to
[reportaproblem.apple.com](https://reportaproblem.apple.com), sign in with your Apple Account and choose to request a
refund, or follow Apple's guide
[Request a refund for apps or content that you bought from Apple](https://support.apple.com/en-us/118223). We cannot
refund App Store purchases ourselves.

### How do I move between the direct download and the Mac App Store version?

The two versions are the same app, distributed in two ways; install one of them on a Mac, not both. They do not share
their own data (settings, search index, API keys), but both open the same library folder:

1. Install the other version and open it.
2. On the welcome screen, choose the **same library folder** as before (in the Mac App Store version, in the folder
   panel that opens). The app finds the existing files and rebuilds its index from them; for a large library this
   takes a while.
3. Set up your AI providers again in Settings › AI Models: enter their **API keys again**, and answer the consent
   question again for cloud providers.

What does not come over: the queue of pending tasks and the usage records, which start again from zero. Search by
meaning returns once the app has indexed the library again in the background.

## Privacy

The [privacy policy]({{ '/privacy/' | relative_url }}) describes what the app stores and sends. We collect no data.

---

<div lang="zh-Hans" markdown="1">

# 支持 {#chinese}

## 获得帮助

在 GitHub 上提交 issue：[github.com/Aliciahan/pubweb-aliciarecorderdesktop/issues](https://github.com/Aliciahan/pubweb-aliciarecorderdesktop/issues)。在那里留言需要一个 GitHub 账号。

**issue 是公开的，任何人都能看到你写的内容。** 不要贴个人信息、录音、逐字稿、笔记、日历内容或 API key。请写清楚你做了什么、发生了什么，以及 App 的版本（设置 › 关于）和 macOS 的版本。
{: .note}

## 常见问题

### 我的录音和笔记存在哪里？

存在你设置 App 时选的资料库文件夹里，例如 iCloud 云盘里的一个文件夹：音频文件、逐字稿、总结和纪要（`.note.md` 文件）、日记和周回顾（`_journal` 文件夹），以及隐藏的 `.alicia` 文件夹里 App 自己关于它们的文件。这些都是普通文件：在 Finder 里就能打开，也可以像其他文件夹一样备份。

App 自己的数据——搜索索引、设置、下载的可选模型和缓存——留在你的 Mac 上：Mac App Store 版在 `~/Library/Containers` 里它的容器中，直发版在 `~/Library/Application Support/AliciaRecorder`。API key 存在 macOS 钥匙串里。索引随时可以从资料库文件夹重建：设置 › 资料库 ›“重建索引…”。

### 什么内容会发给 AI 提供方？怎样停止？

转写、说话人分离和搜索都在你的 Mac 上完成，什么都不发送。总结、纪要、日记、周回顾和问答的回答由你设置的大模型来写，App 发给它的是**文字，从不发送音频**：逐字稿，以及[隐私政策]({{ '/privacy/' | relative_url }}#chinese)第 4.1 节列出的其他内容。向本机和局域网以外的提供方发送任何内容之前，App 会征求你的同意，并写明每项任务发送什么。

要停止或限制发送：

- 在 设置 › AI 模型 里对某个提供方**撤回同意**（“撤回同意”），或者在那里删除这个提供方，它的 API key 也会一并删除。
- 把一段录音**标成“仅本地”**（日期旁边的勾选框，或列表右键菜单里的同名一项）：它就只交给你 Mac 上、局域网里或你设为“按本地对待”的服务器上的模型。
- **只用本地模型**，例如你 Mac 上的 Ollama 或 LM Studio：这样什么都不会离开你的 Mac 或你的网络。

已经发出的文字无法收回，请向提供方申请删除。如果“笔记”只有云端模型，医疗内容的谈话可能在 App 认出它之前就已经发出；隐私政策写了怎样避免。

### 试用和购买怎么算？

这里说的是 Mac App Store 版。App 可以免费下载。你可以在 App 里开始免费的 **15 天试用**，它是一个不收费的 App 内购买项目；试用结束后，一次性购买**完整版**即可解锁，不是订阅。价格显示在 App 里，取自你所在国家或地区的 App Store。

- 试用从你领取的那一刻起算 15 天。它跟着你的 Apple 账户走，所以重装 App 或换一台 Mac 都不会重新开始。
- 没有试用也没有完整版时，你仍然可以打开资料库，阅读、搜索、播放、导出和删除你的录音和笔记，更改设置，重建索引。新录音、导入、转写、写总结和日记、提问，需要试用或完整版。
- 试用结束时正在进行的录音会录完并保存；之后的处理在购买后继续。
- 在另一台 Mac 上或重装之后，在 App 里点**恢复购买**。

试用和购买由 Apple 处理；App 只在你的 Mac 上向 App Store 询问你的 Apple 账户有没有它们。直发版没有试用，也没有购买。

### 怎样退款？

Mac App Store 里的购买是和 Apple 进行的，只有 Apple 能退款。请打开 [reportaproblem.apple.com](https://reportaproblem.apple.com)，用你的 Apple 账户登录后选择申请退款，或者按 Apple 的说明 [Request a refund for apps or content that you bought from Apple](https://support.apple.com/en-us/118223) 操作。App Store 的购买，我们无法自行退款。

### 怎样在直发版和 Mac App Store 版之间换用？

两个版本是同一个 App 的两种发行方式；一台 Mac 上装其中一个就好，不要两个都装。它们不共用各自的数据（设置、搜索索引、API key），但都能打开同一个资料库文件夹：

1. 安装另一个版本并打开它。
2. 在欢迎页面选择**和以前同一个资料库文件夹**（Mac App Store 版会打开一个选择文件夹的面板）。App 会找到已有的文件，并根据它们重建索引；资料库大的话需要一些时间。
3. 在 设置 › AI 模型 里重新设置 AI 提供方：**API key 要重新填**，云端提供方的同意也要重新给。

不会带过来的：排队中的任务和用量记录，它们从零开始。按意思搜索要等 App 在后台重新建好索引之后才恢复。

## 隐私

[隐私政策]({{ '/privacy/' | relative_url }}#chinese)写明了 App 保存什么、发送什么。我们不收集任何数据。

</div>
