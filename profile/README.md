# RogoLabs

Free, open-source sites and tools that take the CVE list apart and publish what they find, each rebuilt from public feeds by GitHub Actions.

RogoLabs is my personal open-source lab. Rogo is Latin for "I ask," which is most of the job: each site below asks one question about vulnerability data and answers it in public, with the code in this org. Jerry Gamblin, [@jgamblin](https://github.com/jgamblin).

## Each site asks one question

| Site | The question it answers | Code |
|---|---|---|
| [CVE.ICU](https://cve.icu) | What is in the CVE list right now? Rebuilt whenever a fresh NVD snapshot lands. | [cve.icu](https://github.com/RogoLabs/cve.icu) |
| [CVEForecast](https://cveforecast.org) | How many CVEs are coming next, overall and per CNA? | [CVEForecast](https://github.com/RogoLabs/CVEForecast) |
| [CVE Floodline](https://cvefloodline.org) | Is a jump in CVE volume rain or a flood? Uses EPSS and CISA KEV to tell them apart. | [cvefloodline.org](https://github.com/RogoLabs/cvefloodline.org) |
| [PatchThis](https://patchthis.app) | What should you patch first? Built from CISA KEV, Metasploit and Nuclei coverage plus high EPSS scores. | [patchthisapp](https://github.com/RogoLabs/patchthisapp) |
| [RBP Tracker](https://rbptracker.org) | Which CVE IDs are cited in public advisories but still sit in Reserved? | [RBP](https://github.com/RogoLabs/RBP) |
| [Ghost CVEs](https://rogolabs.github.io/GhostCVEs/) | Which CVE IDs are already public in commits or advisories while CVE.org lists them as Reserved, or not at all? | [GhostCVEs](https://github.com/RogoLabs/GhostCVEs) |
| [CNA Scorecard](https://cnascorecard.org) | How completely does each CNA fill in its CVE records? | [CNAScoreCard](https://github.com/RogoLabs/CNAScoreCard) |
| [CNAPulse](https://cnapulse.org) | Which CNAs are publishing more, or less, than their own baseline? | [CNAPulse](https://github.com/RogoLabs/CNAPulse) |
| [Consensus Engine](https://rogolabs.github.io/consensus-engine/) | Where do NVD and the GitHub Advisory Database disagree on a CVSS score? | [consensus-engine](https://github.com/RogoLabs/consensus-engine) |
| [CVETime](https://rogolabs.github.io/CVETime/) | How much time passes between CVE publications, globally and per CNA? | [CVETime](https://github.com/RogoLabs/CVETime) |
| [CVE Updates](https://rogolabs.github.io/CVE-Updates/) | How often do CVE records change after they are published? | [CVE-Updates](https://github.com/RogoLabs/CVE-Updates) |
| [SADP Tracker](https://rogolabs.github.io/SADP-Tracker/) | How much are supplier CNAs enriching CVE records through the Supplier ADP program? | [SADP-Tracker](https://github.com/RogoLabs/SADP-Tracker) |

## Tools you run yourself

- [VulnRadar](https://github.com/RogoLabs/VulnRadar): an hourly CVE watchlist on GitHub Actions. Put your vendors and products in `watchlist.yaml`, and a match opens an issue with KEV and EPSS context.
- [quarry](https://github.com/RogoLabs/quarry): a local-first vulnerability hunter for open-source repos on macOS, with sandboxed scanning and draft disclosure advisories.
- Splunk add-ons: [CVE.icu for Splunk](https://github.com/RogoLabs/CVE.icu-Splunk) (the full CVE V5 corpus with EPSS, KEV, SSVC and CVSS, [on Splunkbase](https://splunkbase.splunk.com/app/8395)), [TA-cvelist](https://github.com/RogoLabs/CVE-Splunk-TA) and [TA-epss](https://github.com/RogoLabs/EPSS-Splunk-TA).
- [EPSS-History](https://github.com/RogoLabs/EPSS-History): an archive of the daily EPSS score files from FIRST.

Talk slides live on [rogolabs.net](https://rogolabs.net). Data reviews and build logs live on [jerrygamblin.com](https://jerrygamblin.com).

Every number on these sites comes from a public feed and a script you can read. If one looks wrong, open an issue on that repo and show me. I would rather be corrected than believed.
