Export of Github issues for [OWASP/www-project-machine-learning-security-top-10](https://github.com/OWASP/www-project-machine-learning-security-top-10).

# [\#101 PR](https://github.com/OWASP/www-project-machine-learning-security-top-10/pull/101) `open`: guidelines draft

#### <img src="https://avatars.githubusercontent.com/u/64902909?v=4" width="50">[mik0w](https://github.com/mik0w) opened issue at [2023-08-25 14:38](https://github.com/OWASP/www-project-machine-learning-security-top-10/pull/101):

This PR is related to this issue: https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43

I haven't created Venn's diagram, as I am not sure how should it look, but it's a draft proposition of GUIDELINES document. Looking for feedback :)




-------------------------------------------------------------------------------

# [\#99 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/99) `open`: feat(rendering): make PDF output from Markdown files more presentable
**Labels**: `documentation`, `enhancement`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-24 21:34](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/99):

The Top 10 list is being rendered using Markdown at https://mltop10.info

The site is being rendered using [Quarto](https://quarto.org) and the files from https://github.com/OWASP/www-project-machine-learning-security-top-10/tree/master/docs are mirrored to https://github.com/mltop10-info/mltop10.info

Currently a manual process is run for the https://github.com/mltop10-info/mltop10.info locally to render the HTML and PDF outputs which are stored in https://github.com/mltop10-info/mltop10.info/tree/main/docs and used by Github Pages.

The rendering for PDF is currently using the default method of LaTeX - example at: https://github.com/mltop10-info/mltop10.info/blob/main/docs/OWASP-Machine-Learning-Security-Top-10.pdf

Quarto has a lot of formatting options for generating PDF and this needs to be explored to make the PDF and ePUB formats look more presentable.




-------------------------------------------------------------------------------

# [\#92 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/92) `open`: refactor: rename "neural net reprogramming" to "model poisoning"
**Labels**: `documentation`, `discussions/mltop10`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-20 19:39](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/92):

as per feedback from #87

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-08-20 19:44](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/92#issuecomment-1685375350):

as per comment in #87:

*Corrupting/manipulating model parameters is a general threat, referred to as model poisoning, and is not restricted to neural networks.*


-------------------------------------------------------------------------------

# [\#89 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/89) `open`: [FEEDBACK]: Consider excessive agency
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-08-19 14:11](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/89):

### Type

General Feedback

### What would you like to report?

The LLM top 10 mentions excessive agency, because it is important to limit privileges /autonomy / have oversight over LLM's. This is a general AI problem. 
One could argue whether this is a security risk, and I would argue that it is, because just as AI models are unpredictable, they may also have been manipulated. 
I believe the ML top 10 also needs Excessive agency.

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct




-------------------------------------------------------------------------------

# [\#88 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/88) `open`: [FEEDBACK]: Leaking pipeline is missing
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-08-19 14:07](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/88):

### Type

General Feedback

### What would you like to report?

The risk of leaking training data or other confidentiality issues of the AI pipeline (code, model parameters) are missing. 

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct




-------------------------------------------------------------------------------

# [\#86 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/86) `open`: [FEEDBACK]: Integrate model skewing into data poisoning
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-08-19 14:04](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/86):

### Type

Suggestions for Improvement

### What would you like to report?

[FEEDBACK]: Model skewing requires altering training data, making it a form of data poisoning. Therefore it is probably better to integrate the two threats.

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct




-------------------------------------------------------------------------------

# [\#85 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/85) `open`: [FEEDBACK]: Rename 'Corrupted packages' to 'AI supply chain attacks'
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-08-19 14:02](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/85):

### Type

Suggestions for Improvement

### What would you like to report?

I believe 'Packages' to be a too specific term for the problem of supply chain attacks. Calling it 'supply chain attacks' will make the reader aware of the risk that any external component in the AI pipeline can be manipulated. 
Also, add 'data' as a potential supply chain risk, and refer to 'data poisoning' for that, and also add 'model', referring to the transfer learning attack.

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct




-------------------------------------------------------------------------------

# [\#84 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/84) `open`: [FEEDBACK]: Rename adversarial attack to something less ambiguous
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-08-19 13:58](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/84):

### Type

Suggestions for Improvement

### What would you like to report?

The term adversarial attack usually has a broader definition than the intention of ML01. For example it usually includes data poisoning. 
The intention seems to refer to what is more often called 'evasion attack'. The problem with that term is that it usually means small changes to the input. This is why in the AI guide we used the term 'input manipulation', which is more clear.


### Code of Conduct

- [X] I agree to follow this project's Code of Conduct




-------------------------------------------------------------------------------

# [\#63 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/63) `open`: [Fortnightly] Working Group Meeting - 2023-Aug-17
**Labels**: `meeting`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-16 09:44](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/63):

* Date: [Thursday, August 17 at 0500 UTC](https://dateful.com/convert/utc?t=5am&d=2023-08-02)
* Previous agenda: #42 

## Current agenda

1. General project status - [v0.2 milestone complete](https://github.com/OWASP/www-project-machine-learning-security-top-10/releases/tag/v0.2)
2. Contributions and [current help wanted](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
3. Introductions (for new contributors)

## Discussions

* [Join the OWASP Slack group](https://owasp.org/slack/invite) and the [#project-mlsec-top-10 channel](https://owasp.slack.com/archives/C04PESBUWRZ)
* [Github Discussions](https://github.com/OWASP/www-project-machine-learning-security-top-10/discussions)

## Calendar Event
[Download calendar event (ICS)](https://calendar.google.com/calendar/ical/c_f818ec1e3dea1d4c80cb0f872566eccb82c5df9cc1161f3077f93eafc47889dc%40group.calendar.google.com/public/basic.ics)

#### <img src="https://avatars.githubusercontent.com/u/59761275?u=4e5c4c8a6242383369a6696ab3e21d1df9c875d1&v=4" width="50">[aryanxk02](https://github.com/aryanxk02) commented at [2023-08-17 05:29](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/63#issuecomment-1681638780):

Informative session and a quick update!
cc: @sagarbhure @shsingh


-------------------------------------------------------------------------------

# [\#43 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43) `open`: feat(docs): create a set of guidelines for how to use the Top 10 list
**Labels**: `documentation`, `enhancement`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-02 14:02](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43):

Create a set of guidelines for how to consume the information presented in the Top 10 based on roles
 
Example roles:
- MLOps/MLEng practitioner
- Appsec practitioner

.. etc

#### <img src="https://avatars.githubusercontent.com/u/25385987?u=7cdade85961090394618858dfe721238d54373cd&v=4" width="50">[sagarbhure](https://github.com/sagarbhure) commented at [2023-08-03 04:45](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43#issuecomment-1663282934):

Initial Idea - an umbrella of comprehensive 'nexts-steps.md' resembling a Venn diagram that highlight the intersections between Ethical/Privacy/ML10/LLM10 (i.e. representing efforts from various foundations) which can help tell logical relation between for ex ML and LLM and also there distinct roles and applications where it can also help any practitioner (ops, infra, soft, ml-eng. data-sci etc...) by indicating where they can find relevant resources to support their daily tasks.

The ultimate goal of this initiative is to unify all these efforts under a single umbrella, fostering collaboration and knowledge sharing across different disciplines and specialties. Open to opinion's.

#### <img src="https://avatars.githubusercontent.com/u/2473032?u=b04446601990f318a52534db907414d3d8538bad&v=4" width="50">[edthedev](https://github.com/edthedev) commented at [2023-08-03 14:30](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43#issuecomment-1664094364):

> Initial Idea - an umbrella of comprehensive 'nexts-steps.md' resembling a Venn diagram that highlight the intersections between Ethical/Privacy/ML10/LLM10 (i.e. representing efforts from various foundations) which can help tell logical relation between for ex ML and LLM and also there distinct roles and applications where it can also help any practitioner (ops, infra, soft, ml-eng. data-sci etc...) by indicating where they can find relevant resources to support their daily tasks.
> 
> The ultimate goal of this initiative is to unify all these efforts under a single umbrella, fostering collaboration and knowledge sharing across different disciplines and specialties. Open to opinion's.

@sagarbhure 
Neat. I'm picturing 'swim lanes' for different roles, and process steps linked with arrows in an iterative process flow?

#### <img src="https://avatars.githubusercontent.com/u/25385987?u=7cdade85961090394618858dfe721238d54373cd&v=4" width="50">[sagarbhure](https://github.com/sagarbhure) commented at [2023-08-04 08:17](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/43#issuecomment-1665203955):

> > Initial Idea - an umbrella of comprehensive 'nexts-steps.md' resembling a Venn diagram that highlight the intersections between Ethical/Privacy/ML10/LLM10 (i.e. representing efforts from various foundations) which can help tell logical relation between for ex ML and LLM and also there distinct roles and applications where it can also help any practitioner (ops, infra, soft, ml-eng. data-sci etc...) by indicating where they can find relevant resources to support their daily tasks.
> > The ultimate goal of this initiative is to unify all these efforts under a single umbrella, fostering collaboration and knowledge sharing across different disciplines and specialties. Open to opinion's.
> 
> @sagarbhure Neat. I'm picturing 'swim lanes' for different roles, and process steps linked with arrows in an iterative process flow?

The analogy provided about the guideline is akin to a traffic police officer directing vehicles to take their respective lanes. It's great to see such analogies connecting real-life solutions to problems, as they effectively simplify things and add a new dimension to my thoughts. Thank you for that!

More analogies ?  Would love to see if you are open on contributing to this mission.


-------------------------------------------------------------------------------

# [\#30 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/30) `open`: fix: merge existing body of work from EthicalML https://ethical.institute
**Labels**: `issues/general`, `good first issue`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-07-25 04:39](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/30):

### Type

Documentation Issue Report

### What would you like to report?

There is a comprehensive existing body of work at: https://ethical.institute

The intent would be to review the [current Top 10 list in this project](https://owasp.org/www-project-machine-learning-security-top-10/) and:
- merge content where appropriate
- create new content missing 
- suggest improvements for areas/scope not curently covered

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-07-25 04:42](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/30#issuecomment-1649115556):

Hi @axsaucedo I hope the above comment makes sense. I would love for you to contribute to this given your familiarity and ownership of the https://ethical.institute content.

I see this potentially taking a bit of time as there is a large amount of content at your site to potentially look at merging.

This could also be an opportunity to look at the current Top 10 list categories in this project to see if they need amending.

/cc @sagarbhure @aryanxk02 for visibility


-------------------------------------------------------------------------------

# [\#15 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/15) `open`: feat(docs): create page on calculating severity
**Labels**: `documentation`, `enhancement`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-07-24 00:16](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/15):

Each of the Top 10 items are scored according to [OWASP's Risk Rating Methodology](https://owasp.org/www-community/OWASP_Risk_Rating_Methodology). There should be a page defining how to use the ratings to provide a severity score. This will assist practitioners in knowing 'what to fix' and 'when'.

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-08-24 21:22](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/15#issuecomment-1692428735):

- [ ] create a page showing how risk can be calculated from the top 10 list using the OWASP Risk Rating Methodology
- [ ] add information to each risk with the risk values used


-------------------------------------------------------------------------------

# [\#2 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/2) `open`: fix: merge review from @robvanderveer
**Labels**: `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-04-27 10:07](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/2):

the following is an initial review taken from Slack logs: https://owasp.slack.com/archives/C04PESBUWRZ/p1677192099712519

by @robvanderveer


---
Dear all,
I did a first scan through the list to mainly look at taxonomy. Here are my remarks.
1.
ML01
In 'literature' the term ‘adversarial’ is often used for input manipulation attacks, but also for data poisoning, model extraction etc. Therefore in order to avoid confusion it is probably better to rename the ML01 adversarial attack entry to  input manipulation?
2.
It is worth considering to add ‘model evasion’ aka black box input manipulation to your top 10? Or do you prefer to have one entry for input manipulation all together?
3.
ML03
It is not clear to me how scenarios 1 and 2 work. I must be missing something. Usually model inversion is explained by manipulating synthesized faces until the algorithm behaves like it recognizes the face.
4
ML04
It is not clear to me how scenario 1 works.
Standard methods against overtraining are missing form the ‘how to prevent’ part. Instead the advice is to reduce the training set size - which typically increases the overfitting problem.
5
ML05
Model stealing describes a scenario where an attacker steals model parameters, but generally this attack takes place by ways of black box: gathering input-output pairs and training a new model on it.
6
ML07
I don’t understand exactly how the presented scenario should work. I do know about the scenario where a pre-trained model was obtained that has been altered by an attacker. This matches the description.
7
ML08
Isn’t model skewing the same as data poisoning? If there’s a difference, to me they are not apparent from the scenario and description.
8
ML10 is called Neural net reprogramming but I guess the attack of changing parameters will work on any type of algorithm - not just neural networks. The description also mentions changing the training data, but perhaps that is better left out to avoid confusion with data poisoning?




-------------------------------------------------------------------------------

