Before we submit, finalize, or publicly post a new draft of a paper, the following tasks should be done. These tasks should be added as GitHub Issues, so when a collaborator is asked to "do the production tasks," the collaborator will open (and eventually close) three new GitHub issues, one each for task REF, PROOF, and FACT described below.

### Task [REF]: Check/update references
#### Goals
* A paper is cited in the bibliography if and only if it is referenced in the body of the paper. The fastest way to do this is probably:
 - Search the body of the paper for open parentheses "(", which will bring up references. Make sure that each reference in the body is included in the bibliography.
 - For each bibliography entry, search the body for the author's last name.
* All citations in the body of the paper are formatted consistently
* All bibliography entries are formatted consistently 

#### Deliverables
* A pull request with a corrected and compiled paper tex file
* A single pdf document that highlights (using Acrobat commenting tools) any changes that are substantive enough to require review by Ryan or others. (Post this as an attachment on the GitHub Issue.)

### Task [PROOF]: Proofread spelling, grammar, table references, math, etc.
#### Goals
* Typos, spelling/grammar errors, unclear wording, etc. corrected (don't forget to include table notes, figure notes, footnotes, axis labels, appendices, etc.)
* Follow rules outlined in the [Style Guide](https://github.com/kelloggrk/Kellogg_RA_Manual/wiki/Style-Guides) section
* References to any sections of the paper or tables or figures check out, in the sense that the referenced object exists and seems to have the information promised by the reference
* Titles of sections, tables, figures, etc. are clear, descriptive, and consistent.
* Variable names, notation, and other concepts are used consistently; the same notation is never used to refer to two different things

#### Deliverables
* If you notice a recurring issue, let Ryan/others know immediately via comment thread, and provide examples in the thread. Ryan/others will weigh in with instructions to (i) address the issue throughout; (ii) ignore; (iii) do not change but flag all instances in the final deliverable. Ryan/others will also instruct on whether the Draft Style Guide section of the RA manual should be updated to clarify the issue.
* A single pdf document with all changes/comments clearly marked using Adobe Acrobat's commenting tools. Recurring issues are flagged individually only if requested by Ryan/others per the preceding.
* If there are **obvious** spelling/grammar errors, please go ahead and fix them directly on the tex file; don't include these obvious errors in the comment pdf file.
* Once we have addressed recurrent errors, create a pull request with a corrected and compiled paper tex file.

### Task [FACT]: Check all factual claims made in the paper
#### Goals
* Every quantitative/factual claim made in the paper is supported by (i) a citation, (ii) an entry in a table, (iii) a figure, or (iv) a comment in a tex comment field in the tex file.
 - If a fact is supported by a citation, it is not necessary to check the paper or book we are citing to verify that it contains the fact.
* All tables/figures in the paper pdf are referenced at least once in the paper. 
* All content (tables/figures/discussion) in the online appendix or main appendix is referenced at least once in the paper.
Within each section (tables/figures/discussion) of the online appendix, content appears in the order in which it is referenced in the paper.

#### Deliverables
* When an undocumented claim can be documented, please do so, e.g. by adding a tex comment field to the tex file.
* When you don't know how to document a claim, e.g. because Ryan wrote it and you don't know where the information came from, please compile the paper and use Adobe Acrobat's commenting tools to clearly mark all unsupported claims.


### Task [GALLEY]: Checking galley proofs
#### Goals
* We have flagged all errors in translating our submitted manuscript into the journal's typeset format.
* Note in particular that the goal here is not to proofread the paper (i.e., not to perform the above-listed steps). We presume we will have done that as of the last submission, so the only possible remaining errors are those from typesetting.

#### Deliverables
* A single pdf document that lists all discrepancies between our original typeset manuscript as of the last submission to the journal and the galley proofs using Adobe Acrobat's commenting tools. Pay special attention to the formatting of tables, figures, and equations, as these are where most discrepancies tend to arise.
* In the same pdf document, also comment on anything else that looks like a typo or error that you happen to come across. Note that you should be looking only for discrepancies with respect to the last submission, not doing any other form of proofreading. But if you do notice a probable error along the way it is best to flag it as it may still be possible to correct it.