You should have "atomic commits" on GitHub - that is, a commit should hang together around a single goal or topic. If you have made changes with different purposes since your last commit, it is good practice to add the changes in several logical batches.

Each commit should be made with a message that begins with a reference to the relevant issue(s) and ends with a brief summary of what the commit accomplishes. We reference issues using the syntax `#123` to create a link to issue #123. A commit command could be

`git commit -m "#123 Change something"` (or equivalent in Github desktop)

A good commit message is concise and descriptive. Ideally, the message is a single line of text that explains what you did and why you did it. Below are some examples of good and bad commit messages

* "#123 Modify code.R to add number of observations to main regression table"` [Good]
* `"#123 Modifying code.R"` [Bad, redundant with what git is recording]