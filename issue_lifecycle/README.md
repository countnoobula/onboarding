Issues, PR's and Commits are all different phases of the lifecycle of an incident or feature request.

# Issue - Incident report.
_Issues are either the incident report from the client, or a specification for a feature._

Incident reports can (and should) have an investigative comment from a developer, as to where they believe the problem is, or what may be causing it. Clarifications on the initial report should also be documented in the relevant issue so that we maintain a source of truth for the incident. These clarifications may come from discussions in slack, over the phone, or any other sources - the important part is that they exist in the issue.

As incident reports are often received from the client, it can sometimes be lacking in description. For example:
```My shower is broken, I have no idea what is going on.```

Sometimes they may be a bit more descriptive:
```My computer isn't working, I think the bios is out of date.```

Or a more developer friendly version of an issue:
```I am not receiving the password-reset email. I have waited 30 minutes, and still nothing.```

It is up to you as a developer to investigate and understand the client's requirements. The issue comments are there to better understand the client's problem or issue.

In regards to specifications of features or changes to be implemented, these will generally be more specific in either a user story, epic, or draft. These may require input from a developer to assist with establishing timeline estimations, and clarifying certain specifications and requirements.

It is important to note that issues can be created by anyone and that the quality of the product is the responsibility of the product team. If a developer notices an inconsistency or an oddity, raise a discussion about it through an issue.

---

# PR - Implementation report.
_This is what the technician gives his boss when he gets back to the office._

The PR is an implementation report, also known as a summary, that explains the implementation at a technical level. It is a summary of all steps taken to complete a task, or a part of a task, it also comments on the final outcome and what may still be outstanding.

The PR should also reference the relevant issue (as per the PR template). If the PR fully resolves the relevant issue- it should be preceded with a [magic GitHub word](https://help.github.com/en/articles/closing-issues-using-keywords) 

An example of an PR message is:
```I went out to the house, and discovered that the bios was out of date. The reason for the issue was that the bios had not been updated in years. Once the bios was updated the problem was resolved.```

In a more developer-friendly example:
```
There were a few entries in Sentry where JobOffer discount and cash_discount caused calculation problems because the value inserted into the database was NaN.
This resolves it by adding stricter validation (cash_discount, discount and meet should be integer), and corrects existing NaN values for discount and cash_discount.
Relevant Sentry issue: ...
```



---

# Commit - Outlines of steps taken.
_These are the steps that the technician took to resolve the issue._

Your commits should be contextual step by step procedures as to how you achieved it. Commits should also follow the [7 rules](https://chris.beams.io/posts/git-commit/) for [good commit messages](https://www.git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project#Commit-Guidelines).

In the case of the technician from earlier, his steps were: 
```
1. Arrive at the client's house
2. Take out motherboard
3. Update motherboard bios
```

The title of the commit should be imperative, and be able to be substituted into the following sentence structure:
```If applied, this commit will _commit title here_```

In a more developer-friendly example of a good commit title:
```
Add Docker to getting started documentation
```

The commit body should be describing the what and why. Code is generally self-documenting to a degree, but to save the future maintainer time, the body should make clear the reasons why you made the change in the first place, the way things worked before the change (and what was wrong with that), the way they work now, and why you decided to solve it the way you did.

---

Here are some examples of good commit messages

![PR#2617](https://i.imgur.com/0Unylal.png)
![PR#2659](https://i.imgur.com/yc91bnx.png)
