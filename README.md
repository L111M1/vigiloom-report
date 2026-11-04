# Drug safety research report library

[Open the report library](https://l111m1.github.io/vigiloom-report/)

The shared landing page offers Chinese and English versions of three completed studies:

| Study | English | Chinese |
|---|---|---|
| SGLT2 inhibitors (four-drug study) | [Read](reports/sglt2/report.html) | [阅读](reports/sglt2/report_zh.html) |
| Cetirizine | [Read](reports/cetirizine/report.html) | [阅读](reports/cetirizine/report_zh.html) |
| Pregabalin | [Read](reports/pregabalin/report.html) | [阅读](reports/pregabalin/report_zh.html) |

Each report includes symptom search, collapsible navigation, source links, an internal-link return control and a link back to the report library. Reports remain self-contained HTML. The publication process adds navigation without changing clinical findings or calling APIs.

Root `report.html` and `report_zh.html` preserve existing pregabalin links. Previously shared root URLs containing report anchors continue to the English pregabalin report.

`publication.json` records source runs, source HTML hashes, the generator commit and SHA256 hashes of all published HTML. Files are published as UTF-8/LF.

To update the website, regenerate reports in the private local runs, update `config/report_library.json` in the generator repository, then run `tools/publish_reports.py --output <this checkout>`. Review and push this publication checkout separately. The script does not run research or make Git changes itself.

[Generator repository](https://github.com/L111M1/vigiloom)

The [evidence audit](evidence-audit.md) is a historical note dated 1 November and is not a publication status summary for the full library.
The sticky symptom finder also contains a visible three-study switcher. Switching studies preserves the reading language; the current study is highlighted. Print-report buttons have been removed.
