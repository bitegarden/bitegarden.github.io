---
layout: post
title: How to export a PDF from SonarQube Community Build
description: Export project metrics with the Web API or download a PDF with bitegarden Report. Compare both options and see a sample report.

permalink: export-pdf-sonarqube-community-build
spanish: exportar-pdf-sonarqube-community-build

cover: /img/posts/2026-11-26-export-pdf-sonarqube-community-build_en.png
---

With the [bitegarden Report Plugin](https://marketplace.bitegarden.com/product/bitegardenReport), you can download a PDF directly from your project in **SonarQube Community Build**. Choose an executive summary to share the project status or an issue breakdown to review individual findings with your team.

[Sonar's native PDF reports](https://docs.sonarsource.com/sonarqube-server/user-guide/viewing-reports/pdf-reports) are available from **SonarQube Server Enterprise Edition** and focus mainly on new code and Quality Gate conditions. In Community Build, you can also retrieve project metrics with the Web API and create your own PDF.

<h2>How to build a report with the Web API</h2>

This option works well when you need a few metrics for a release review or want to use an existing reporting template. The API returns the data as JSON. You choose which metrics to include and how to present them in the PDF.

1. Run an analysis and find your project key in SonarQube. Create a user token with access to the project and make it available to your shell as `SONAR_TOKEN`.
2. Request the metrics you want to share. The example below asks for coverage, duplicated lines density and lines of code for WebGoat. Replace the example URL and project key with those from your instance. Check the [Web API documentation](https://docs.sonarsource.com/sonarqube-community-build/extension-guide/web-api) for authentication and the endpoints available in your version.

```bash
curl --fail --silent --show-error --get \
  --header "Authorization: Bearer ${SONAR_TOKEN}" \
  --data-urlencode 'component=org.owasp.webgoat:webgoat' \
  --data-urlencode 'metricKeys=coverage,duplicated_lines_density,ncloc' \
  --output sonarqube-metrics.json \
  'https://sonarqube.example.com/api/measures/component'
```

Open `sonarqube-metrics.json` and look for `component.measures`. Copy the values you need into a spreadsheet or document template, add the project name and analysis date, then export it to PDF. For recurring reports, you can use the same request to feed a template or an existing reporting tool.

<h2>How to download a PDF with the bitegarden plugin</h2>

Before installing the plugin, check the marketplace listing for a release that supports your version of Community Build.

1. Download the compatible plugin version and follow the [installation and setup guide](/sonarqube-report-documentation).
2. Open a project that has already been analysed and go to **More > Reporting**.
3. Download the **Executive PDF Summary** for a quick project review. Choose an issue breakdown report if the reader needs more detail about the findings.

See the [sample WebGoat executive report (PDF)](/pdf/sonarqube-sample-executive-report-webgoat.pdf) to check how bitegarden presents project metrics in a document you can share.

[Start your free 14-day trial](https://marketplace.bitegarden.com/download/download-form/55){: .btn .btn-primary .btn-call-to-action}

<h2>Which option fits your project?</h2>

| What you need | Where to start |
| --- | --- |
| A few metrics for a spreadsheet or an internal template | Use the Web API and export your finished document to PDF. |
| A PDF from the project interface for a review or handover | Use the bitegarden plugin and choose the level of detail. |
| A built-in PDF and you already have Enterprise Edition | Check what the native report covers for your project. |

<br>

If you also need an editable file, see our [guide to exporting reports to PDF and Excel](/export-reports-sonarqube-pdf-excel).

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
