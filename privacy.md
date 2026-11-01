# Privacy Policy — KenjaGrid

**Effective date: November 1, 2026**

**The short version: KenjaGrid collects nothing.** There are no accounts, no analytics, no ads, and no tracking. Your workbooks never leave your device — the only network traffic the app ever makes is when **you** use the built-in AI assistant, and those requests go directly to the AI provider **you** configured. We run no AI service and see none of that traffic.

KenjaGrid is a spreadsheet app for macOS, Windows, Linux and BSD (with a browser build via WebAssembly), developed by KenjaHub ("we", "us"). It is free, open-source software, and its source code is public — you can verify everything in this policy yourself. This policy explains what happens to your data when you use the app.

## 1. Data we collect

None. KenjaGrid does not transmit any personal data to us, and does not share data with any third party on our behalf.

In particular, KenjaGrid does **not** include:

- user accounts or sign-in
- analytics, telemetry, or crash-reporting SDKs
- advertising or ad tracking of any kind
- third-party trackers

## 2. Your workbooks stay on your device

Everything KenjaGrid does with your workbooks happens locally on your device:

- **Creating, editing, calculating, formatting, charting, printing and exporting all run on your machine.**
- **Workbooks are never uploaded.** There is no server, no sync, no cloud — workbooks and exports are written wherever you choose on your disk.

## 3. The AI assistant — the only network traffic

KenjaGrid includes a built-in AI assistant that can answer questions about the active workbook. It uses **your** model, not ours (bring your own key):

- **You configure the endpoint.** The assistant speaks to any OpenAI-compatible endpoint you set up in the app — OpenAI, DeepSeek, Qwen, or a local server such as Ollama or LM Studio.
- **Requests go directly from your device to that endpoint.** We run no AI service and no proxy: your questions, your workbook content and your key never pass through us, and we could not see them if we wanted to.
- **What a request contains:** your message, the recent conversation, and the workbook content the assistant reads through its inspection tools — a workbook or sheet summary, cell values, or a text search. By default the assistant can only look: read-only is the default, and it cannot modify your workbook unless you explicitly switch to one of the edit modes.
- **Your API key** is stored only in the app's settings file on your device, and is sent only to the base URL you configured, as an authorization header. For a local server you can leave it empty (keyless mode), and then nothing is sent.
- **The conversation lives in memory only.** It is kept per document, closing the app or the document clears it, and nothing is ever written to disk.
- **In the browser (WebAssembly) build, the AI assistant is unavailable** — the web app makes no AI requests at all.
- **Once your data reaches the provider you chose, their privacy policy governs it.** We do not choose, vet or endorse providers — pick one you trust.

## 4. Data stored on your device

The following data is stored only on your device, under your full control:

- **Workbooks and exports** — the files you create, open or export stay wherever you saved them; KenjaGrid keeps no copy
- **App settings** — including your AI model profiles: base URL, model id and API key, kept in the app's settings file
- **Log files** — the app writes a local log (`gridcraft.log` in its logs folder) to help you debug problems; it stays on your machine, is size-capped, and is never sent to us (you can attach it to a bug report yourself if you choose to)

Uninstalling the app removes the app and its local settings. Your workbooks are yours and remain untouched.

## 5. Network access and the local agent interface

KenjaGrid itself initiates no network traffic — there is no account check, no update ping, no telemetry. The only internet traffic the app ever sends is an AI-assistant request that **you** triggered, delivered to the endpoint **you** configured. Updates are delivered by GitHub Releases or your package manager, not by us.

KenjaGrid is agent-native, and its automation interfaces are strictly local: the MCP server talks over standard input/output, and the optional JSON control channel listens only on your own machine (127.0.0.1) and only when you explicitly start the app with it enabled. Agents work on your workbooks the way you do — on your machine. Nothing in these interfaces contacts the internet or us.

## 6. Children

KenjaGrid is a general-purpose productivity tool and is not directed at children. Since the app collects no data at all, no data of children is collected either.

## 7. Your control

Because everything lives on your device, you are in full control at any time: open, copy, export or delete your workbooks like any other file, remove your saved models and keys in the Manage Models settings, delete the log files, or uninstall the app to erase its settings.

## 8. Changes to this policy

If we change this policy, we will post the updated version on this page with a new effective date.

## 9. Contact

- Email: [kenjasoft@kofukuai.com](mailto:kenjasoft@kofukuai.com)
- GitHub: <https://github.com/KenjaHub>

---

# 隐私政策 — KenjaGrid（简体中文）

**生效日期：2026 年 11 月 1 日**

**简而言之：KenjaGrid 不收集任何数据。**没有账号、没有统计、没有广告，也没有追踪。你的工作簿从不出你的设备——应用唯一会产生的网络流量，是**你**使用内置 AI 助手的时候，而那些请求直接发往**你自己配置**的 AI 服务商。我们不运营任何 AI 服务，也看不到那些流量。

KenjaGrid 是一款电子表格应用，支持 macOS、Windows、Linux 和 BSD（另有 WebAssembly 浏览器版本），由 KenjaHub（下称「我们」）开发。它是免费的开源软件，源代码公开——本政策中的每一条你都可以亲自验证。本政策说明你使用本应用时，你的数据会发生什么。

## 1. 我们收集的数据

无。KenjaGrid 不会向我们传输任何个人数据，也不会代表我们与任何第三方共享数据。

具体而言，KenjaGrid **不包含**：

- 用户账号或登录
- 统计分析、遥测或崩溃报告 SDK
- 任何形式的广告与广告追踪
- 第三方追踪器

## 2. 工作簿留在你的设备上

KenjaGrid 对你的工作簿所做的一切，都在你的设备本地完成：

- **创建、编辑、计算、格式化、制图、打印与导出，全部在你的设备上运行。**
- **工作簿从不上传。**没有服务器、没有同步、没有云端——工作簿与导出文件只写入你在磁盘上选择的位置。

## 3. AI 助手——唯一的网络流量

KenjaGrid 内置一个 AI 助手，可以就当前活动工作簿回答问题。它用的是**你自己的**模型，而不是我们的（自带密钥，BYOK）：

- **端点由你配置。**助手通过 OpenAI 兼容接口与你设置的任意端点通信——OpenAI、DeepSeek、Qwen，或 Ollama、LM Studio 等本地服务。
- **请求从你的设备直接发往该端点。**我们不运营任何 AI 服务、也没有任何代理：你的问题、工作簿内容与密钥都不经过我们，我们想看也看不到。
- **请求包含的内容：**你的消息、最近的对话，以及助手通过检查工具读取的工作簿内容——工作簿或工作表概要、单元格数值，或文本搜索结果。默认情况下助手只能查看：只读是默认模式，除非你显式切换到某一种编辑模式，否则它不能修改你的工作簿。
- **你的 API 密钥**只保存在你设备上的应用设置文件里，且只以授权头的形式发往你配置的基础 URL。使用本地服务时可以留空（无密钥模式），此时什么都不会发送。
- **对话仅存于内存。**它按文档保存，关闭应用或文档即被清除，任何内容都不会写入磁盘。
- **在浏览器（WebAssembly）版本中，AI 助手不可用**——Web 版不会发出任何 AI 请求。
- **数据到达你选择的服务商之后，适用他们的隐私政策。**我们不推荐、不审查、也不背书任何服务商——请选择你信任的服务商。

## 4. 存储在你设备上的数据

以下数据仅存储在你的设备上，完全由你掌控：

- **工作簿与导出文件**——你创建、打开或导出的文件留在你保存它们的位置；KenjaGrid 不保留任何副本
- **应用设置**——包括你的 AI 模型配置：基础 URL、模型 ID 与 API 密钥，保存在应用设置文件中
- **日志文件**——应用会在本地写一份日志（日志文件夹中的 `gridcraft.log`），方便你排查问题；它只留在你的电脑上、有大小上限，绝不会发给我们（是否附到 bug 报告里，由你自己决定）

卸载应用会移除应用及其本地设置。你的工作簿属于你，不会被触碰。

## 5. 网络访问与本地 Agent 接口

KenjaGrid 自身不发起任何网络流量——没有账号验证、没有更新探测、没有遥测。应用唯一发出的互联网流量，是**你**触发的一次 AI 助手请求，发往**你**配置的端点。更新由 GitHub Releases 或你的包管理器提供，而非我们。

KenjaGrid 对 Agent 友好，而它的自动化接口严格限于本地：MCP 服务器通过标准输入输出通信；可选的 JSON 控制通道只监听你自己的机器（127.0.0.1），并且只有在你显式以启用方式启动应用时才会开启。Agent 和你一样，在你的机器上处理你的工作簿。这些接口都不会连接互联网，也不会连接我们。

## 6. 儿童

KenjaGrid 是一款通用效率工具，不面向儿童。由于应用完全不收集数据，自然也不会收集任何儿童数据。

## 7. 你的掌控

因为一切都保存在你的设备上，你始终拥有完全的掌控：像操作任何普通文件一样打开、复制、导出或删除你的工作簿；在「管理模型」设置中删除已保存的模型与密钥；删除日志文件；或卸载应用以清除其设置。

## 8. 政策变更

如果我们修改本政策，会在本页发布更新版本，并注明新的生效日期。

## 9. 联系方式

- 邮箱：[kenjasoft@kofukuai.com](mailto:kenjasoft@kofukuai.com)
- GitHub：<https://github.com/KenjaHub>

---

# プライバシーポリシー — KenjaGrid（日本語）

**発効日：2026 年 11 月 1 日**

**要点：KenjaGrid は何も収集しません。**アカウントも、分析も、広告も、トラッキングもありません。お客様のワークブックが端末の外へ出ることはありません。アプリが通信を行うのは、内蔵 AI アシスタントを**お客様ご自身が**使ったときだけで、そのリクエストは**お客様が設定した** AI プロバイダーへ直接送られます。当社は AI サービスを運営しておらず、その通信を見ることもできません。

KenjaGrid は macOS・Windows・Linux・BSD 対応（WebAssembly によるブラウザ版もあり）のスプレッドシートアプリで、KenjaHub（以下「当社」）が開発しました。無料のオープンソースソフトウェアであり、ソースコードは公開されています。本ポリシーの内容は、お客様ご自身で確認できます。本ポリシーは、アプリご利用の際にお客様のデータがどう扱われるかを説明するものです。

## 1. 収集するデータ

なし。KenjaGrid は当社へいかなる個人データも送信せず、当社のために第三者へデータを共有することもありません。

とくに、KenjaGrid には以下のものは**含まれません**：

- ユーザーアカウントやサインイン
- アナリティクス、テレメトリー、クラッシュレポート SDK
- いかなる形態の広告および広告トラッキング
- サードパーティのトラッカー

## 2. ワークブックはお客様の端末に残ります

KenjaGrid がワークブックに対して行うすべての処理は、お客様の端末上でローカルに実行されます：

- **作成・編集・計算・書式設定・チャート・印刷・書き出しは、すべてお客様の端末上で動作します。**
- **ワークブックがアップロードされることは一切ありません。**サーバーも、同期も、クラウドもなく、ワークブックや書き出しファイルはお客様が選んだ場所に保存されます。

## 3. AI アシスタント——唯一のネットワーク通信

KenjaGrid には、作業中のワークブックについて質問に答える内蔵 AI アシスタントがあります。使うのは**お客様の**モデルであり、当社のものではありません（BYOK——自分のキーを持参する方式）：

- **エンドポイントはお客様が設定します。**アシスタントは、アプリ内で設定した OpenAI 互換エンドポイントと通信します。OpenAI、DeepSeek、Qwen、あるいは Ollama・LM Studio などのローカルサーバーでもかまいません。
- **リクエストはお客様の端末からそのエンドポイントへ直接送られます。**当社は AI サービスもプロキシも運営していません。お客様の質問・ワークブックの内容・キーが当社を経由することはなく、当社が見ることもできません。
- **リクエストに含まれるもの：**お客様のメッセージ、最近の会話履歴、そしてアシスタントが検査ツールで読んだワークブックの内容——ワークブックやシートの概要、セルの値、テキスト検索の結果です。既定ではアシスタントは閲覧のみ可能です。読み取り専用が既定であり、お客様が明示的に編集モードのひとつに切り替えない限り、ワークブックを変更することはできません。
- **API キー**はお客様の端末内のアプリ設定ファイルにのみ保存され、設定されたベース URL に認証ヘッダーとして送信されるだけです。ローカルサーバーでは空にでき（キーレスモード）、その場合は何も送信されません。
- **会話はメモリ上にのみ存在します。**ドキュメントごとに保持され、アプリやドキュメントを閉じると消去され、ディスクに書き込まれることは一切ありません。
- **ブラウザ（WebAssembly）版では AI アシスタントは利用できません。**Web 版は AI リクエストを一切送信しません。
- **データがお客様の選んだプロバイダーに到達した後は、そのプロバイダーのプライバシーポリシーが適用されます。**当社はプロバイダーの選定・審査・推薦を行いません。信頼できるプロバイダーをお選びください。

## 4. 端末に保存されるデータ

以下のデータはお客様の端末にのみ保存され、完全にお客様の管理下にあります：

- **ワークブックと書き出しファイル**——作成・開いた・書き出したファイルは保存した場所にそのまま残り、KenjaGrid はコピーを保持しません
- **アプリ設定**——AI モデルプロファイル（ベース URL、モデル ID、API キー）を含む設定は、アプリの設定ファイルに保存されます
- **ログファイル**——アプリは問題調査のためローカルにログ（ログフォルダー内の `gridcraft.log`）を書きます。端末内にのみ保存され、サイズ上限があり、当社へ送られることは一切ありません（バグ報告に添付するかどうかはお客様が決めます）

アプリをアンインストールすると、アプリとそのローカル設定は削除されます。ワークブックはお客様のものであり、手つかずのまま残ります。

## 5. ネットワークアクセスとローカルエージェントインターフェース

KenjaGrid 自身は、ネットワーク通信を一切開始しません。アカウント確認も、更新確認も、テレメトリーもありません。アプリが送信する唯一のインターネット通信は、**お客様が**実行した AI アシスタントのリクエストで、**お客様が**設定したエンドポイントへ送られます。アプリの更新は当社ではなく GitHub Releases またはお使いのパッケージマネージャーから配信されます。

KenjaGrid はエージェントフレンドリーですが、その自動化インターフェースは厳密にローカルです。MCP サーバーは標準入出力で通信し、オプションの JSON 制御チャネルは、明示的に有効にして起動した場合に限り、お客様の端末（127.0.0.1）でのみ待ち受けます。エージェントはお客様と同じく、お客様の端末上でお客様のワークブックを扱います。これらのインターフェースがインターネットや当社に接続することはありません。

## 6. 児童

KenjaGrid は汎用の生産性ツールであり、児童向けに作られたものではありません。アプリはまったくデータを収集しないため、児童のデータも収集されません。

## 7. お客様の管理

すべてが端末内に存在するため、データの管理権限は常に完全にお客様側にあります。ワークブックはほかのファイルと同じように開く・コピー・書き出し・削除ができ、「モデルの管理」設定から保存済みのモデルとキーを削除したり、ログファイルを削除したり、アプリをアンインストールして設定を消去したりできます。

## 8. 本ポリシーの変更

本ポリシーを変更する場合は、このページに新しい発効日付きの更新版を掲載します。

## 9. お問い合わせ

- メール：[kenjasoft@kofukuai.com](mailto:kenjasoft@kofukuai.com)
- GitHub：<https://github.com/KenjaHub>

---

© 2026 KenjaHub
