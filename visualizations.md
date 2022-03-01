# Badger visualizations

Badger is a tool that provides several visualizations of open-source contributions that the company and it's employees have made.

The Tretton37 badger sources it's data from GitHub. It's scope is set to the organization [tretton37](https://github.com/tretton37).

Following are some example visualizations that the tool generates.

> Note: You can also get `.svg` graphics by replacing the `.png` extension in the URL.

At the moment, the home for the Badger (and other OSS tools we use) is here: `https://oss-tools.azurewebsites.net`. You can check out the API specification by navigating to the `/swagger` enndpoint.

---

Markdown: `![IndividualContributors](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualContributors&all=false&limit=10)`

![IndividualContributors](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualContributors&all=false&limit=10)

| Parameter | Description                                                                                                  |
| --------- | ------------------------------------------------------------------------------------------------------------ |
| all       | Include all contributions in calculations. Defaults to only [whitelisted](#project-whitelist) contributions. |
| limit     | Limit results to the number specified. No limit is imposed by default                                        |

---

Markdown: `![IndividualContributorSpecifics](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualContributorSpecifics&all=false&limit=10)`

![IndividualContributorSpecifics](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualContributorSpecifics&all=false&limit=10)

| Parameter | Description                                                                                                  |
| --------- | ------------------------------------------------------------------------------------------------------------ |
| all       | Include all contributions in calculations. Defaults to only [whitelisted](#project-whitelist) contributions. |
| limit     | Limit results to the number specified. No limit is imposed by default                                        |

---

Markdown: `![ProjectContributions](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=ProjectContributions&project=bunit)`

![ProjectContributions](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=ProjectContributions&project=bunit)

| Parameter | Description                                                    |
| --------- | -------------------------------------------------------------- |
| project   | The project statistics to display. This parameter is required. |

---

Markdown: `![ProjectEmployeeContributions](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=ProjectEmployeeContributions&project=bunit&limit=10)`

![ProjectEmployeeContributions](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=ProjectEmployeeContributions&project=bunit&limit=10)

| Parameter | Description                                                           |
| --------- | --------------------------------------------------------------------- |
| project   | The project statistics to display. This parameter is required.        |
| limit     | Limit results to the number specified. No limit is imposed by default |

---

Markdown: `![IndividualProjects](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualProjects&all=true&limit=10)`

![IndividualProjects](https://oss-tools.azurewebsites.net/badger/table-badge.png?type=IndividualProjects&all=true&limit=10)

| Parameter | Description                                                                                                  |
| --------- | ------------------------------------------------------------------------------------------------------------ |
| all       | Include all contributions in calculations. Defaults to only [whitelisted](#project-whitelist) contributions. |
| limit     | Limit results to the number specified. No limit is imposed by default                                        |

---

Markdown: `![TotalCommits](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalCommits&all=true)`

![TotalCommits](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalCommits&all=true)

| Parameter | Description                                                                                                  |
| --------- | ------------------------------------------------------------------------------------------------------------ |
| all       | Include all contributions in calculations. Defaults to only [whitelisted](#project-whitelist) contributions. |

---

Markdown: `![TotalCommits](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalCommits&project=piranha.core)`

![TotalCommits](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalCommits&project=piranha.core)

| Parameter | Description                                                    |
| --------- | -------------------------------------------------------------- |
| project   | The project statistics to display. This parameter is required. |

---

Markdown: `![TotalPrs](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalPrs&project=bunit)`

![TotalPrs](https://oss-tools.azurewebsites.net/badger/badge.png?type=TotalPrs&project=bunit)

| Parameter | Description                                                    |
| --------- | -------------------------------------------------------------- |
| project   | The project statistics to display. This parameter is optional. If not specified unfiltered result set will be returned.|

---

## Project whitelist

We get the projects we contribute to by looking at what out public members contribute to. This can lead to a large number of contributions to different projects that may or may not be connected to our organized efforts. Therefore we impose a limitation.

By default, contributions will be calculated across whitelisted projects only. Currently the following projects are whitelisted:

| Project      |
| ------------ |
| bUnit        |
| piranha.core |

> Note: you can turn off this limitation by setting the query parameter `all=true` in any badge url.
