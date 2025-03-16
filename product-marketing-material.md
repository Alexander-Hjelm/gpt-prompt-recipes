Substitute the variables in all text after the token "$BEGIN PROMPT$". with the following values:

$(productName)              = Jira AzureDevOps Migrator
$(productDescription)       = A migration tool that migrates issues from Jira to work items in Azure DevOps.
$(companyName)              = Solidify
$(includeKSPs)              = [YES]
$(optionalExtraTextInput)   = "
Azure DevOps Backup Tool provides a set of pipeline tasks that backs up Azure DevOps data as json files to a local file directory."

The extension consist of the following tasks:

- **Azure DevOps Backup Tool: Export** - Run export jobs via a pipeline task. Save the downloaded files to a local file area or network file share.
- **Azure DevOps Backup Tool: Import** - Run import jobs via a pipeline task. Read the files from a local file area or network file share.

Omit all lines from the prompt that start with the token "- [NO]" (without quotation marks). Include any lines that start with the token "- [YES]", but delete the "- [YES]" token itself.

Return only the resulting prompt and no details about the substituted variables.

$BEGIN PROMPT$

Write a marketing text for our product.

- Product name: $(productName)
- Company name: $(companyName)

Description of the product: $(productDescription).

- $(includeKSPs) Include a list of key selling points under the title "Why choose us?".

Here is some existing documentation on the tool that you can use for inspiration:

$(optionalExtraTextInput)