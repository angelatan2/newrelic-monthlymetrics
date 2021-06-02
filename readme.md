# newrelic-monthlymetrics
Script to gather metrics about how the teams are functioning and how the community is contributing.

1. set your GitHub API token as an environment variable

`export GITHUB_TOKEN='your_token_value'`
Note: This is not the token name but the value itself.

2. Configure your teams in the teams.json file

3. Run pip3 install requests 
This will install requests library package if you don't already have it.

4. Run the script using `python3 metrics.py`

This script makes the following assumptions

1. You're using GitHub teams to indicate who is a team member and who is an external contributor.
2. New bugs get the label `needs-triaged` to indicate the bug has not yet been reviewed by the team. Once the review has occurred, the label should be removed.
