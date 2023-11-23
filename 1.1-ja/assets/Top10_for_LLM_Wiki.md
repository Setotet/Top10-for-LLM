## Top10 for LLM (日本語版) Wiki

### 目的

このWikiページは、1.1-jaドラフト版の作成プロジェクトの進捗状況をまとめたものです。1.1-jaドラフト版翻訳・更新作業は、[このgithubレポジトリ](https://github.com/Setotet/Top10-for-LLM/tree/1.1-ja) 上で行っており、このWikiは、作業の進行に同期し最新の進捗状況を掲載しています。

OWASP Top 10 for Large Language Model Applications 全体の情報は、
[英語Wiki](https://owasp.org/www-project-top-10-for-large-language-model-applications/)に掲載されています。英語版PDFは、[このサイト](https://llmtop10.com/)でも公開しています。

### 日本語版の1.0から1.1への進捗状況

| Commit diff | Commit message |
| ----------- | --------------------- |
| [R51122_224150](https://github.com/Setotet/Top10-for-LLM/commit/95588cd42e3b6a926eb754aad5e4ea532339f9c7) | Fix section title and increase precision to .4f |
| [R51122_171146](https://github.com/Setotet/Top10-for-LLM/commit/4d6866e1e44e4994d581848ca814459895bf9858) | Apply 1_1_vulns/_template.md |
| [R51121_215619](https://github.com/Setotet/Top10-for-LLM/tree/1.1-ja/1.1-ja/1.0-ja_orig) | Prepare for 1.1-ja |


| Chapter title | Links to chapter diff | BLEU score |
| ------------- | --------------------- | ---------- |
| PromptInjection | [LLM-01](URL) | 0.9636 |
| InsecureOutputHandling | [LLM-02](URL) | 0.9510 |
| TrainingDataPoisoning | [LLM-03](URL) | 0.9644 |
| ModelDoS | [LLM-04](URL) | 0.9446 |
| SupplyChainVulnerabilities | [LLM-05](URL) | 0.9509 |
| SensitiveInformationDisclosure | [LLM-06]() | 0.9524 |
| InsecurePluginDesign | [LLM-07](URL) | 0.9543 |
| ExcessiveAgency | [LLM-08](URL) | 0.9658 |
| Overreliance | [LLM-09](URL) | 0.9481 |
| ModelTheft | [LLM-10](URL) | 0.9554 |

### BLEU scoreについて

BLEU scoreは自然言語処理で広く用いられている2つの文章の類似度を示す 0.0~1.0 (inclusive) の小数で、1は完全に一致する、0は完全に異なることを意味します。日本語1.1版の作成は日本語1.0版をベースとし、英語の1.0版から1.1版への変更箇所（以下を参照）に沿って、翻訳・更新していきますから、出発点ではベースと同じ、すなわち、BLEU scoreは1.0で、変更が進むにつれて減少していきますから、日本語1.1版の翻訳・更新の進捗を一つの数値で表すと解釈することができます。

しかし、0になることはありません。0.5以下になることもないでしょう。いくつになったら1.1版への更新が終了するかということを一意に定めることはできませんが、おおまかな目安として、英語の1.0版から1.1版への更新では以下に示すように、章ごとに見ると0.54から0.90の間にあり、平均は0.7315です。英語版のBLEU scoreが小さい（変更が多い）章は日本語版でも小さくなる（翻訳・更新が多くなる）傾向を示すであろうと思われます。

### BLEU scoreの変化

翻訳・更新は当該githubレポジトリへcommitすることで行っています。commit毎のBLEU scoreの実測値を示す経時折線グラフを以下に示します。

**To Be Added**

### 日本語版の1.0から1.1へのタスク・リスト

- [x] 1.1-jaレポジトリ作成
- [x] Top10_for_LLM-Wiki.md 作成
- [ ] 1.1-ja翻訳グロッサリー作成
- [ ] LLM01-Prompt_Injections 翻訳・更新
- [ ] LLM02-Insecure_Output_Handling 翻訳・更新
- [ ] LLM03-Training_Data_Poisoning 翻訳・更新
- [ ] LLM04-Model_Denial_of_Service 翻訳・更新
- [ ] LLM05-Supply_Chain_Vulnerabilities 翻訳・更新
- [ ] LLM06-Sensitive_Information_Disclosure 翻訳・更新
- [ ] LLM07-Insecure_Plugin_Design 翻訳・更新
- [ ] LLM08-Excessive_Agency 翻訳・更新
- [ ] LLM09-Overreliance 翻訳・更新
- [ ] LLM10-Model_Theft 翻訳・更新
- [ ] TBA 1
- [ ] TBA 2
...
- [ ] Fullwhite paper 1.1-ja 作成
- [ ] OWASP本体のレポジトリに挙げる

### 英語版の1.0から1.1への更新

英語版は1.0と1.1が[このgithubレポジトリ](https://github.com/OWASP/www-project-top-10-for-large-language-model-applications)にあります。英語版の1.0から1.1への変更は以下のようになっています。

| Chapter Title | Links to chapter diff | BLEU score |
| ------------- | --------------------- | ---------- |
| PromptInjection | [LLM-01](https://github.com/talesh/llm_top_ten_diffs/commit/f1ffe5cf96833fb15a585277996fd2cc05401396) | 0.7166 |
| InsecureOutputHandling | [LLM-02](https://github.com/talesh/llm_top_ten_diffs/commit/015539a321537a77cff3d5210b01b9d23ccba1d0) | 0.5495 |
| TrainingDataPoisoning | [LLM-03](https://github.com/talesh/llm_top_ten_diffs/commit/c1fa2664bf3dc078c458861fd45ac37d30953d00) | 0.5637 |
| ModelDoS | [LLM-04](https://github.com/talesh/llm_top_ten_diffs/commit/3d67a52b5d6962fb12ab9fbb4714ebdd2914f3b4) | 0.8589 |
| SupplyChainVulnerabilities | [LLM-05](https://github.com/talesh/llm_top_ten_diffs/commit/ff8f66336df56d27371c31da49c329f76937de13) | 0.6617 |
| SensitiveInformationDisclosure | [LLM-06](https://github.com/talesh/llm_top_ten_diffs/commit/96826c14f0fcf9ac0b8d85229349377eae9e27ff) | 0.7325 |
| InsecurePluginDesign | [LLM-07](https://github.com/talesh/llm_top_ten_diffs/commit/3742a4a4a246a3fec61dd110ec9ba921ff968d4f) | 0.7530 |
| ExcessiveAgency | [LLM-08](https://github.com/talesh/llm_top_ten_diffs/commit/9d0d60ecdf7901546b6c39e04618dcba22fafda9) | 0.8931 |
| Overreliance | [LLM-09](https://github.com/talesh/llm_top_ten_diffs/commit/3800d56c741d0c0df0759be36dbdfe50288e0b90) | 0.7547 |
| ModelTheft | [LLM-10](https://github.com/talesh/llm_top_ten_diffs/commit/6a2f97f85ccc20059f32e72535a2ee3bf6e94454) | 0.8309 |

### Reference Links

1. [BLEU Wikipedia](https://en.wikipedia.org/wiki/BLEUL)
1. [Foundations of NLP Explained — Bleu Score and WER Metrics](https://towardsdatascience.com/foundations-of-nlp-explained-bleu-score-and-wer-metrics-1a5ba06d812b)
