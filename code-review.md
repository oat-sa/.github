# Code Review Process

How does a developer typically do code reviews?

Code reviews can be performed in many ways. Sometimes, it is as informal as one developer walking over to another developer’s desk to look at some code together. Other times, teams review code together in groups.
Let’s imagine a developer at OAT, and let us call him Mike. Mike was just assigned a ticket and now wants feedback from her peers.
What should Mike do before starting a code review?
Mike can proceed and involve the team into a small session (15m) of design review where he will showcase the decision he wants to take before

## Best Practises 

Mike should take a look at the following [guide](https://oat-sa.atlassian.net/wiki/spaces/OAT/pages/11338720/Development+Workflow+with+Github)[ ](https://oat-sa.atlassian.net/wiki/spaces/OAT/pages/11338720/Development+Workflow+with+Github)and make sure his work is according to the guide.
How does Mike start a code review at OAT?
Well, as said, Mike is ready to get some feedback. Therefore, he first prepares the code for review. This step includes that he opens a draft pull
request, that allows her to preview the code change.
The code review tool performs some diffing tasks that help Mike to see exactly which changes he has done.

**Tools**:

***PHP***
 - <https://www.jetbrains.com/help/phpstorm/using-php-code-sniffer.html>
- <https://www.jetbrains.com/help/phpstorm/using-php-mess-detector.html>
- <https://www.jetbrains.com/help/phpstorm/using-php-cs-fixer.html>
- <https://www.jetbrains.com/help/phpstorm/using-phpstan.html>
- <https://www.jetbrains.com/help/phpstorm/using-psalm.html>

***JavaScript***

- <https://www.jetbrains.com/help/phpstorm/eslint.html>
- <https://www.jetbrains.com/help/phpstorm/jslint.html>


## Author self-review

- [ ] New code is covered by tests (if applicable)
- [ ] Tests are running successfully (old and new ones) on my local machine (if applicable)
- [ ] New code is respecting code style rules
- [ ] New code is respecting best practices
- [ ] New code is not subject to concurrency issues (if applicable)
- [ ] Feature is working correctly on my local machine (if applicable)
- [ ] Acceptance criteria are respected
- [ ] Pull request title and description are meaningful
- [ ] Pull request's target is not `master`
- [ ] The changes in this PR meet the user experience and goals outlined in the content design plan.
- [ ] For REST API content, I've verified that endpoints, parameters, and responses are correct and work as expected and provided curl samples below.

## Review request

### Template:
```
Ticket: https://oat-sa.atlassian.net/browse/LEAD-123

#### What's Changed

- Introduced a new feature called `foobar`.

#### TODO

- [x] Unit tests
- [x] E2E tests
- [ ] Update composer with packages

#### Dependencies PRs

- https://github.com/oat-sa/tao-core/

#### How to test

- Explain here how to test or make a small demo to our team how this
```
### Docs Content review

_Give Docs Content any extra context, highlight areas for them to consider in their review, and ask them questions you need answered to ship the PR._

### Technical review

_Ping in technical reviewers, asking them to review whether content is technically accurate and right for the audience._
_Highlight areas for them to consider in their review and ask them questions you need answered to ship the PR._
_The reviewers are often other developers, but can also include other stakeholders, such as dev-ops engineers, UI experts, or also managers._
_Some reviewers are selected for their expertise, others are selected in order to stay informed about a coming change._

### GitHub etiquette
In order to make our PR merged faster please follow below best practices.

#### Checklist

**OAT software engineering department policy**. 
Each person that reviewing a PR is required to apply below checklist into their PR comment and mark boxes when applied.
```
- [ ] New code is covered by tests (if applicable)
- [ ] Tests are running successfully (old and new ones) on my local machine (if applicable)
- [ ] New code is respecting code style rules
- [ ] New code is respecting best practices
- [ ] New code is not subject to concurrency issues (if applicable)
- [ ] Feature is working correctly on my local machine (if applicable)
- [ ] Acceptance criteria are respected
- [ ] Pull request title and description are meaningful
- [ ] Pull request's target is not `master`
```

#### Protip
To get have the checklist available at a glance, add it to [your](https://github.com/settings/replies)[ ](https://github.com/settings/replies)[GitHub](https://github.com/settings/replies)[ ](https://github.com/settings/replies)[profile’s](https://github.com/settings/replies)[ ](https://github.com/settings/replies)[saved](https://github.com/settings/replies)[ ](https://github.com/settings/replies)[replies](https://github.com/settings/replies)

#### Commenting
A good habit is to use [conventional](https://conventionalcomments.org/)[ ](https://conventionalcomments.org/)[comments](https://conventionalcomments.org/)[ ](https://conventionalcomments.org/)to properly emphasize the meanings.

##### Labels
We strongly suggest using the following labels:

| labels      |                                                                                                                                Description                                                                                                                                |
|-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| praise      |                                 Praises highlight something positive. Try to leave at least one of these comments per review. *Do not* leave false praise (which can actually be damaging). *Do* look for something to sincerely praise.                                  |
| nitpick:    |                                                                                          Nitpicks are trivial preference-based requests. These should be non-blocking by nature.                                                                                          |
| suggestion: |     Suggestions propose improvements to the current subject. It's important to be explicit and clear on what is being suggested and why it is an improvement. Consider using patches and the blocking or non-blocking decorations to further communicate your intent.     |
| issue:      | Issues highlight specific problems with the subject under review. These problems can be user-facing or behind the scenes. It is strongly recommended to pair this comment with a suggestion. If you are not sure if a problem exists or not, consider leaving a question. |
| todo:       |                                          TODO's are small, trivial, but necessary changes. Distinguishing todo comments from issues: or suggestions: helps direct the reader's attention to comments requiring more involvement.                                          |
| question:   |                                      Questions are appropriate if you have a potential concern but are not quite sure if it's relevant or not. Asking the author for clarification or investigation can lead to a quick resolution.                                       |
| thought:    |                                Thoughts represent an idea that popped up from reviewing. These comments are non-blocking by nature, but they are extremely valuable and can lead to more focused initiatives and mentoring opportunities.                                 |
| chore:      |            Chores are simple tasks that must be done before the subject can be “officially” accepted. Usually, these comments reference some common process. Try to leave a link to the process description so that the reader knows how to resolve the chore.            |
| typo:       |                                                                                                    Typo comments are like todo:, where the main issue is a mispelling.                                                                                                    |
| polish:     |                                                   Polish comments are like a suggestion, where there is nothing necessarily wrong with the relevant content, there's just some ways to immediately improve the quality.                                                   |
| polish:     |                                                   Polish comments are like a suggestion, where there is nothing necessarily wrong with the relevant content, there's just some ways to immediately improve the quality.                                                   |
| quibble:    |                                                                             Quibbles are very much like nitpick:, except it does not conjure up images of lice and animal hygiene practices.                                                                              |


##### Resolving Comments*

A comment may be resolve by an author of comment when:
 - comment has been applied in code
 - the issue has been answered
 - the subject has been explained
 - A comment may be resolved by PR owner when a comment has been applied in code.

### Content changes

[PR on internal uat](LINK HERE)
_Give a high-level overview of the changes in your PR and how they support the overall goals of the PR. Share links to important articles or changes in source and on staging. If your PR is large or complex, use a table to highlight changes with high user impact._


### Pull request size
_Accoding to the team this should be a common consensus but the recommendation is not to have a bigger PR then 20 pages as this will increase the code review time So best method is to take the code and see if you as the developer can read and understand it in 1hour and then split it into multiple PR’s if required in order to facilitate a faster approval and merge._

### Notes

_PSR-12 or equivalent for FE or Go._
_Discuss test failures, versioning issues, or anything else reviewers should know to consider the overall user experience of the PR._
