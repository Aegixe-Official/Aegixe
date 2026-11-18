# Audit Report Lookup Guide

[中文](audit-report-lookup.zh-CN.md) · [Open tool](https://aegixe.com/ai_edit_query_new/) · [Index](../README.md)

Scope: the Chinese AEGIXE audit report lookup web interface. Workflow checked on 12 November 2026.

## 1. Enter a project name

1. Open the lookup and enter the formal project name in “请输入项目名称”, rather than a wallet address, transaction hash or arbitrary ticker.
2. Check the spelling and click “查询”. Wait for the result page to finish loading.
3. Verify the queried object and final state. The process labels for scanning, manual review, logic validation and final reports do not establish that a particular project completed an audit.

## 2. When a report link is available

1. Use “立即下载” only when a valid download link remains available after loading completes.
2. After downloading, verify the project, issuer, date, revision, network, full contract addresses and reviewed commit inside the original report.
3. Compare it with the current deployment and inspect scope, findings, fixes and retest status. See the [report checklist](audit-report-checklist.md).

A download button or filename alone authenticates neither the report's relationship to a project nor a claim that the project is safe. This repository does not include detection reports, client audit reports or sample results.

## 3. When no report is found

The check observed “未找到该报告，重新查询” and a no-match status referring to the entered name. In this situation:

1. Use the retry link to return to the form and check the formal name and spelling.
2. If still unmatched, use the [official contact entry](https://aegixe.com/contact-us-form/) to ask how to obtain the report.
3. Record “lookup did not return a match”. This does not establish that the project has never been audited.

Default content during loading is not the final search result. Wait for a stable state; do not cite a report from a briefly visible download link.

## 4. Common issues and scope

- **Duplicate names or tickers:** distinguish projects by the report's network, addresses and code version.
- **Broken download:** record time, name and page state; retry later or contact the team. Do not substitute a different project's report.
- **Upgraded project:** an old report does not automatically cover changed code, privileges or deployment.

Non-empty submission, navigation, the no-match state and download-link presentation were checked. PDF download and content matching have not completed verification. This guide explains lookup and verification, rather than certifying a report or a project's safety.
