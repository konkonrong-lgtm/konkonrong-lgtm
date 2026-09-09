# キム・ソンフン / Sunghun Kim

**関西学院大学 工学部｜2028年卒業予定｜ソフトウェアエンジニア志望**

実際の業務で使われるWebアプリと、開発者向けツールを作っています。利用者の声をもとにした改善や、既存のコードを読んで原因を調べ、修正・テストまで進めることに取り組んでいます。

- **業務アプリ開発：** 飲食店向けシフト管理システムを開発し、実運用のフィードバックをもとに継続改善
- **公式OSSへの貢献：** SalesforceのVS Code拡張に不具合修正と回帰テストを提出し、採用・マージ
- **開発者向けツール：** Salesforce Multi-Frameworkの事前検証CLI「mf-check」を開発し、npmで公開

## 主なプロジェクト・貢献

### 飲食店向けシフト管理システム

9店舗・約130名が所属する飲食店運営組織に向けて設計・開発したWebアプリです。この数字は対象組織の規模であり、アクティブ利用者数ではありません。

シフト提出、店舗・役割ごとの管理、人員不足の可視化、配置補助を実装。既存の業務で必要なExcel出力にも対応し、店長からのフィードバックをもとに画面や運用を改善しています。

**技術：** Next.js / TypeScript / Supabase / PostgreSQL / Vercel

[ポートフォリオ・設計資料](https://github.com/konkonrong-lgtm/shift-management-system-portfolio) · [スタッフ向けデモ](https://demo-shift.vercel.app/s/demo) · [店長向けデモ](https://demo-shift.vercel.app/manager/demo/login)（デモ用パスワード：`1111`）

### Salesforce公式OSS — salesforcedx-vscode

Salesforce以外のプロジェクトで `.cls` ファイルを開くと、Apex Language Serverが起動し、不要なファイルが生成される問題を調査しました。

原因を追跡し、Salesforceプロジェクトかどうかを確認する処理と回帰テストを追加。提出した **PR #7973** は、Salesforce側のCI・レビュー用の **PR #7976** に取り込まれ、作者情報を保持したままマージされました。

[提出したPR #7973](https://github.com/forcedotcom/salesforcedx-vscode/pull/7973) · [採用・マージされたPR #7976](https://github.com/forcedotcom/salesforcedx-vscode/pull/7976)

### mf-check — Salesforce Multi-Framework事前検証CLI

「デプロイに成功してもアプリが使える状態にならない」という問題をきっかけに開発しました。

UI Bundleと内部アプリ・Experience Cloudの参照関係、ローカルの権限設定、対象orgのスキーマに対するGraphQL互換性を検査します。外部 `.graphql` ファイルとSalesforce SDKの静的inline `gql` に対応し、誤検知の削減を重視しています。

**技術：** TypeScript / Babel AST / GraphQL / Vitest / GitHub Actions  
npmで公開し、自動テストとCIで継続的に検証しています。

[ソースコード・使い方](https://github.com/konkonrong-lgtm/mf-check) · [npm](https://www.npmjs.com/package/@konkonrong/mf-check)

## その他の取り組み

- **セキュリティ報告：** Salesforce Product Securityに問題を報告し、再現できたとの連絡を受けています。技術的な詳細は公開可否が確認できるまで非公開にしています。
- **開発中：** 飲食店向けの食材・レシピ・原価管理システム。

## 使用技術

- **言語：** TypeScript / JavaScript / Python
- **Web・データベース：** React / Next.js / Supabase / PostgreSQL
- **開発・検証：** Git / Salesforce CLI / Vitest / GitHub Actions

<details>
<summary>English profile</summary>

## About me

I'm Sunghun Kim, an engineering student at Kwansei Gakuin University in Japan, expecting to graduate in 2028 and pursuing a software engineering career.

I build web applications for real operational needs and tools for developers. My work includes improving products through user feedback, investigating existing codebases, and writing fixes with regression tests.

### Selected work

**Restaurant Shift Management System**  
Built a web application for a restaurant organization spanning 9 stores and approximately 130 staff members. These figures describe the organization, not active usage. The system covers shift submission, staffing shortages, assignment assistance, and Excel export, with ongoing improvements based on operational feedback.

Next.js / TypeScript / Supabase / PostgreSQL / Vercel

[Portfolio and design documents](https://github.com/konkonrong-lgtm/shift-management-system-portfolio) · [Staff demo](https://demo-shift.vercel.app/s/demo) · [Manager demo](https://demo-shift.vercel.app/manager/demo/login) (demo password: `1111`)

**Salesforce OSS — salesforcedx-vscode**  
Investigated unintended Apex Language Server startup outside Salesforce projects, added a project guard, and wrote regression tests. My [PR #7973](https://github.com/forcedotcom/salesforcedx-vscode/pull/7973) was adopted into [PR #7976](https://github.com/forcedotcom/salesforcedx-vscode/pull/7976) and merged with author credit preserved.

**mf-check — Multi-Framework preflight CLI**  
Created an npm-published CLI to check UI Bundle linkage, local access metadata, and GraphQL compatibility with a target Salesforce org. Supports external `.graphql` files and static inline Salesforce SDK `gql`, with a focus on reducing false positives.

TypeScript / Babel AST / GraphQL / Vitest / GitHub Actions

[Repository](https://github.com/konkonrong-lgtm/mf-check) · [npm](https://www.npmjs.com/package/@konkonrong/mf-check)

### Other work

- Reported a security issue that Salesforce Product Security confirmed it could reproduce. Technical details remain private pending disclosure clearance.
- Currently building a restaurant ingredient, recipe, and cost management system.

</details>
