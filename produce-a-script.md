Substitute the variables inside the prompt with the following values:

$(language)              = Powershell
$(requirements)          =
 - Do a rest api call to fetch all repositories from an azure devops instance
 - Write the repository names, repo created date and information about the latest commit to a json file.
 - Get the latest commit via a rest API call
 - The output to the json file should be handled in a separate function
$(params)                = $ADO_ORG_URL, $ADO_USERNAME, $ADO_PAT
$(output)                = A json file containing the API response
$(authorName)            = Alexander Hjelm
$(authorEmail)           = nick.nertova@gmail.com
$(includeHelpSection)    = [NO]
$(includeHeadingComment) = [YES]
$(includeUsageExamples)  = [YES]
$(includeAuthor)         = [YES]
$(includeDate)           = [YES]

Omit all lines from the prompt that start with the token "- [NO]" (without quotation marks). Ignore any occurences of the token "- [YES]"

Return only the resulting prompt and no details about the substituted variables.

$BEGIN PROMPT$

Generate a self contained CLI script using all text after the token "$BEGIN PROMPT$".

- Programming language: $(language)
- Requirements on the script: $(requirements)
- Input parameters: $(params)
- Output: $(output)

- $(includeHelpSection) Include a help section with the --help argument.
- $(includeHeadingComment) Include a helpful comment at the top of the script that describes what the script does
- $(includeUsageExamples) Include a usage example at the top of the script
- $(includeAuthor) Include the author: $(authorName), $(authorEmail) at the top of the script
- $(includeDate) Include today's date at the top of the script