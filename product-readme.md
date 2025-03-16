Substitute the variables in all text after the token "$BEGIN PROMPT$". with the following values:

$(repoName)                         = my-repository
$(language)                         = Powershell
$(appDescription)                   = a CLI utility that fetches all repositories from an Azure DevOps instance and saves the results as a json file.
$(includeContributionGuidelines)    = [YES]
$(includeUsageExample)              = [YES]

Omit all lines from the prompt that start with the token "- [NO]" (without quotation marks). Include any lines that start with the token "- [YES]", but delete the "- [YES]" token itself.

Return only the resulting prompt and no details about the substituted variables.

$BEGIN PROMPT$

Create a readme.md file for developers for my application.

Description of the application: $(appDescription).

The repository name is $(repoName).

- $(includeContributionGuidelines) Include contribution guidelines. A contributor may raise a PR to the main branch and tag an active developer for review.
- $(includeUsageExample) Include a usage example.