Export of Github issues for [OWASP/www-project-machine-learning-security-top-10](https://github.com/OWASP/www-project-machine-learning-security-top-10).

# [\#194 PR](https://github.com/OWASP/www-project-machine-learning-security-top-10/pull/194) `open`: chore: github issues archive

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-12-18 04:11](https://github.com/OWASP/www-project-machine-learning-security-top-10/pull/194):

- chore: github issues archive
- chore: github issues archive





-------------------------------------------------------------------------------

# [\#189 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/189) `open`: [FEEDBACK]: Include a page with a brief descriptions of each of the vulnerabilities
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/64902909?u=756899683e78c4e336cc1e8a6b7584bc6b508200&v=4" width="50">[mik0w](https://github.com/mik0w) opened issue at [2023-11-23 12:08](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/189):

### Type

Suggestions for Improvement

### What would you like to report?

For example in Top10 for LLM there's this page with a summary of each of the vulnerabilities, which I think would be pretty useful to have in Top10 for ML as well. 

Sometimes  when you e.g. work on some slides for a presentation, you just want to get a short summary of each of the vulnerabilities. In my opinion including such a page in Top10 for ML would be an improvement: 

![summary](https://github.com/OWASP/www-project-machine-learning-security-top-10/assets/64902909/0bc2b1c8-43a0-4a5d-b549-71cf83e897c1)

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-12-18 04:07](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/189#issuecomment-1859518422):

Hi @mik0w is the suggestion to create a summary page? Or to look at enhacing the introductory sections within each of the ML risks so that they can be used as a summary? Or both? 

In either case I think this is a good idea, let me get started on it.


-------------------------------------------------------------------------------

# [\#188 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/188) `open`: [FEEDBACK]: Include MLOps vulnerabilties somewhere in the Supply Chain Security category 
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/64902909?u=756899683e78c4e336cc1e8a6b7584bc6b508200&v=4" width="50">[mik0w](https://github.com/mik0w) opened issue at [2023-11-17 10:26](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/188):

### Type

Suggestions for Improvement

### What would you like to report?

**Context**
One of the parts of the supply chain in modern ML systems is MLOps software - like i.e. MLFlow, Prefect etc. Those systems are vulnerable to classic web based attacks and they seem to be "misconfured by default". I've described it here: https://hackstery.com/2023/10/13/no-one-is-prefect-is-your-mlops-infrastructure-leaking-secrets/ or here: https://github.com/logspace-ai/langflow/issues/1145 

**Suggestion for improvement**
I'd suggest including MLOps-related vulnerabilities in the ML06 (or maybe in some other categories as well? I am open for suggestions). 

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct

#### <img src="https://avatars.githubusercontent.com/u/25385987?u=7cdade85961090394618858dfe721238d54373cd&v=4" width="50">[sagarbhure](https://github.com/sagarbhure) commented at [2023-11-28 05:42](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/188#issuecomment-1829141861):

In my view it should be in ML06, However is should be better renamed with ML from AI supply chain i believe to keep ourself distinct, How would you recommend adding these in the existing ML06, keeping the attacks generic to other packages

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-12-18 04:06](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/188#issuecomment-1859517344):

Hi @mik0w I definitely think we should look at including the ecosystem of MLOps software. I am not sure that it all falls within  supply chain though. Keen to hear your thoughts on this.


-------------------------------------------------------------------------------

# [\#187 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/187) `open`: [FEEDBACK]: Sync attack names between LLMT10 and MLT10 where appropriate
**Labels**: `issues/general`, `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/795878?u=d704fd433504e531d707c517cdb6ff75bdf20372&v=4" width="50">[kapsolas](https://github.com/kapsolas) opened issue at [2023-11-16 22:16](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/187):

### Type

Suggestions for Improvement

### What would you like to report?

I would like to make the suggestion that we consolidate the terms used in the LLM and ML top 10 documents.

Many of the top 10 items in each are closely related or even the same.
Where possible, the same term should be used (i.e. Model Theft vs Model Stealing, Data Poisoning Attack vs Training data Poisoning).

Thanks!

### Code of Conduct

- [X] I agree to follow this project's Code of Conduct

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-12-18 04:03](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/187#issuecomment-1859515638):

Hi @kapsolas apologies for the delay in responsing.

Will definitely look to changing "Model Stealing" to "Model Theft". 

In terms of "Data Poisoning v Training data poisoning" I would like to defer to @yodap-dg 

Typically in research papers it is referred to as "Data Poisoning" and I agree that the use case is largely around the training data itself.

What are your thoughts @yodap-dg?


-------------------------------------------------------------------------------

# [\#182 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/182) `open`: fix: merge review from @harrietf
**Labels**: `issues/triage`, `review needed`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-31 18:00](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/182):

[Harriet Farlow](https://www.linkedin.com/in/harriet-farlow-654963b7/) sent through her feedback via mail.

Uploading Word doc and also outputting to Markdown in this issue to track.

Feedback in Word doc: [OWASP Top Ten Feedback.docx](https://github.com/OWASP/www-project-machine-learning-security-top-10/files/13219930/OWASP.Top.Ten.Feedback.docx)



Output in Markdown from Word doc below:
---
**General feedback - the list and the home page**

I think this is great! Some feedback below:

-   I would also add something about these kinds of mitigations being
    risk-based, and that each organisation should make a risk-based
    assessment of which specific attacks are more likely to be employed
    against their models, how impactful the ramifications would be (ie.
    would they lose massive amounts of PII or would someone just get a
    bad customer experience) and then decide on their ML security
    posture from there.

-   I would also highlight some of the reasons why ML systems are
    different to traditional cyber systems (ie. ML systems are
    probabilistic while cyber systems are rules based, ML systems learn
    and evolve while cyber systems are more static). From an
    organisational perspective this means that it is unfair to expect
    cyber security professionals to automatically know how best to
    secure ML systems, and that there should be investment in training
    and/or the creation of new roles

-   I would also add a comment about the terminology here being ML
    security vs AI security. Clarify the difference between ML and AI
    (ie. AI is a broader set of technologies while ML refers
    specifically to the AI sub-field of ML models). For example, I
    usually refer to my work as AI Security to be more encompassing of
    an audience who is used to hearing about AI, but most of what I talk
    about is actually ML security. Adding something here about these
    terms would be useful for non-ML folk.

**Some questions before I give feedback on these things**

-   Is the intention of the top 10 list that it is also ordered so that
    #1 is most threatening, or is it unordered?

-   What is the methodology/reference for the risk factor values under
    each threat? (I know it comes from the specific scenarios, but is it
    meant to also be representative of 'common' ways of implementing the
    attack? Because it could be very different and might be interpreted
    as generic)

**ML01:2023 Input Manipulation Attack**

-   Where Adversarial Attacks are referenced in the intro, I usually see
    this referred to as an Adversarial Example instead and this language
    would be more consistent. I'm also not sure what it means by saying
    it's an umbrella term, what are the other attacks underneath this
    umbrella?

-   The list Adversarial Training, Robust Models, Input Validation are
    all good to include but could be rephrased to be mutually exclusive
    (ie. the Robust Models section references both Adversarial Training
    and Input Validation as the way to make models robust). You could
    start with Robust Models first and still mention that those other
    two techniques are some ways to make model robust, but is also
    dependent on good data quality (clean data, good feature
    engineering, complete data), model selection (having to choose an
    appropriate balance between accuracy and interpretability, which are
    usually trade-offs), considering ensemble methods instead of a
    single model (ie. you get results from multiple models as a way of
    checking and validation output). You can then into system level
    security measures (input validation) and process-based security
    measures (incorporating adversarial training).

-   Love the scenarios, that really helps to put it in perspective.

**ML02:2023 Data Poisoning Attack**

-   Would be worth including more here in the 'about' section around how
    this normally happens (an organisation's data repository could have
    new data added, or existing data altered), why it works (an ML
    model's heavy reliance on training data and the fact that it needs
    LOTS of it, which means it's also very hard to spot if it has been
    tampered with), who is likely to do this (someone either needs
    access to the data repository if the model is trained on internal
    data only in which case an insider threat scenario is more likely,
    or if the model learns from 'new' data fed from the outside like a
    chatbot that learns off inputs without validation (ie. Tay) then
    this is a much easier attack) etc. Also clarify how this is
    different to the cyber security challenge of just keeping data
    secure (ie. it's more about the statistical distribution of the data
    than the likelihood of data breach).

-   The 'how to prevent this section' is great, and adding more info
    beforehand might help make it clearer as to why these measures are
    important, and why the measure to secure data is for different
    reasons than traditional cyber security threat models.

-   Again, great examples. You could add something like a chatbot or
    social media model here to underscore how publicly injected data is
    also a risk here.

**ML03:2023 Model Inversion Attack & ML04:2023 Membership Inference
Attack**

-   These two attacks could be clarified as to exactly how they're
    different, and depending on how you expect someone might use the Top
    10, you could consider combining them. For example, they both leak
    information about data used to train the model but model inversion
    is about leaking any data, and membership inference is more about
    seeing if a specific piece of data was used. Or you could clarify
    that they are separate based on the different controls used to
    prevent it (ie. is the focus on differentiation here the goal of
    attack, or the means of securing it)

-   Model inversion - you could explain what it means to
    'reverse-engineer' in this context. Ie. it is more about targeted
    prompting than reverse engineering in a cyber context. This would
    also explain why the suggested controls (ie. input verification)
    work.

**ML05:2023 Model Stealing**

-   This is good! Again, I think a longer description would be helpful.

**ML06:2023 AI Supply Chain Attacks**

-   Yes, love that this is included!

-   Why are we switching from ML to AI here?

**ML07:2023 Transfer Learning Attack**

-   This is interesting.. In my mind this is more an AI misuse issue
    than an AI security issue, but it really depends on the scenario I
    think. Could be worth clarifying here.

**ML08:2023 Model Skewing**

-   This also seems the same as the data poisoning attack.. It's not
    clear how they're different. Usually when I saw model skewing the
    attack is based on being able to change the model outcome without
    actually touching the training data.. Would be worth clarifying
    here.

**ML09:2023 Output Integrity Attack**

-   Again, this attack overlaps a lot with other attacks already listed
    that aim to impact the output, it's almost more of an umbrella term
    in my mind. Or it could be different but it depends on how an
    organisation creates its threat model. The controls mentioned here
    are good though, so it's worth clarifying why this is listed as a
    different attack and if it's based on the controls suggested (which
    would also apply to the other attacks listed).

**ML10:2023 Model Poisoning**

-   Yes, this is good, and worth adding a bit more about how this can
    happen (ie. direct alteration of the model through injection, the
    interaction with hardware here and how this can be done in memory
    etc)






-------------------------------------------------------------------------------

# [\#178 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/178) `open`: feat(docs): create a GLOSSARY page of commonly used terms
**Labels**: `documentation/general`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-31 16:48](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/178):

Machine Learning has a lot of terminology that may be new to people. Need to create a glossary page of commonly used terms.

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-31 16:56](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/178#issuecomment-1787613865):

- [glossary page](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/tab_glossary.md)
- [rendered on site](https://owasp.org/www-project-machine-learning-security-top-10/#div-glossary)


-------------------------------------------------------------------------------

# [\#172 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/172) `open`: chore(admin): assign owner(s) for ML10 Model Poisoning
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:31](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/172):

- [ ] Assigned Lead Contributor for ML10
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML10 will also be assigned to the cheatsheet - ref: #158 




-------------------------------------------------------------------------------

# [\#171 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/171) `open`: chore(admin): assign owner(s) for ML09 Output Integrity Attack
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:30](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/171):

- [ ] Assigned Lead Contributor for ML09
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML09 will also be assigned to the cheatsheet - ref: #157 




-------------------------------------------------------------------------------

# [\#170 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/170) `open`: chore(admin): assign owner(s) for ML08 Model Skewing
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:29](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/170):

- [ ] Assigned Lead Contributor for ML08
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML08 will also be assigned to the cheatsheet - ref: #156 




-------------------------------------------------------------------------------

# [\#167 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/167) `open`: chore(admin): assign owner(s) for ML05 Model Stealing
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:27](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/167):

- [ ] Assigned Lead Contributor for ML05
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML05 will also be assigned to the cheatsheet - ref: #153 




-------------------------------------------------------------------------------

# [\#166 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/166) `open`: chore(admin): assign owner(s) for ML04 Membership Inference Attack
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:26](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/166):

- [ ] Assigned Lead Contributor for ML04
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML04 will also be assigned to the cheatsheet - ref: #152 




-------------------------------------------------------------------------------

# [\#165 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/165) `open`: chore(admin): assign owner(s) for ML03 Model Inversion Attack
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:25](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/165):

- [ ] Assigned Lead Contributor for ML03
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML03 will also be assigned to the cheatsheet - ref: #151 




-------------------------------------------------------------------------------

# [\#163 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/163) `open`: chore(admin): assign owner(s) for ML01 Input Validation Attack
**Labels**: `help wanted`, `documentation/risks`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 06:21](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/163):

- [ ] Assigned Lead Contributor for ML01
- [ ] Update CODEOWNERS with contributor details

Ideally the Lead Contributor for ML01 will also be assigned to the cheatsheet - ref: #147 




-------------------------------------------------------------------------------

# [\#158 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/158) `open`: feat(docs): create a cheatsheet for ML10 Model Poisoning
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 05:01](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/158):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#157 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/157) `open`: feat(docs): create a cheatsheet for ML09 Output Integrity Attack
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 05:01](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/157):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#156 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/156) `open`: feat(docs): create a cheatsheet for ML08 Model Skewing
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 05:00](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/156):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#155 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/155) `open`: feat(docs): create a cheatsheet for ML07 Transfer Learning Attack
**Labels**: `enhancement`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 05:00](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/155):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-11-15 03:32](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/155#issuecomment-1811755511):

adding @techiemac as potential lead to this due to his request for taking lead on the risk document.

adding @sagarbhure and @shsingh as backup


-------------------------------------------------------------------------------

# [\#154 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/154) `open`: feat(docs): create a cheatsheet for ML06 AI Supply Chain Attacks
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 05:00](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/154):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-31 17:01](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/154#issuecomment-1787621593):

adding @mik0w as potential lead to this due to his request for taking lead on the risk document.

adding @sagarbhure and @shsingh as backup


-------------------------------------------------------------------------------

# [\#153 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/153) `open`: feat(docs): create a cheatsheet for ML05 Model Stealing
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 04:59](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/153):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#152 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/152) `open`: feat(docs): create a cheatsheet for ML04 Membership Inference Attack
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 04:59](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/152):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#151 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/151) `open`: feat(docs): create a cheatsheet for ML03 Model Inversion Attack
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 04:58](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/151):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)




-------------------------------------------------------------------------------

# [\#150 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/150) `open`: feat(docs): create a cheatsheet for ML02 Data Poisoning Attack 
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 04:57](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/150):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-11-02 10:04](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/150#issuecomment-1790425001):

adding @yodap-dg as potential lead to this due to his request for taking lead on the risk document.

adding @sagarbhure and @shsingh as backup


-------------------------------------------------------------------------------

# [\#147 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/147) `open`: feat(docs): create a cheatsheet for ML01 Input Manipulation Attacks 
**Labels**: `enhancement`, `help wanted`, `documentation/cheatsheets`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:48](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/147):

- [ ] Is there existing cheatsheets at [OWASP Cheatsheets](https://cheatsheetseries.owasp.org/Glossary.html)
- [ ] If there is an existing cheatsheet, does it need updating at the source to cater for machine learning use cases?
- [ ] Is there a need for a new cheatsheet topic?
- [ ] Add existing or new cheatsheet as a reference to the Top 10 risk document

Example Cheatsheet: [Input Validation Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Input_Validation_Cheat_Sheet.md)

Example of Top 10 risk referencing cheatsheets: [ML01 Input Manipulation Attacks - Cheatsheets](https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/docs/cheatsheets/ML01_2023-Input_Manipulation_Attack-Cheatsheet.md)






-------------------------------------------------------------------------------

# [\#145 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/145) `open`: feat(docs): create a recorded demo of ML10 Model Poisoning
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:26](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/145):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#144 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/144) `open`: feat(docs): create a recorded demo of ML09 Output Integrity Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:26](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/144):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#143 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/143) `open`: feat(docs): create a recorded demo of ML08 Model Skewing
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:25](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/143):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#142 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/142) `open`: feat(docs): create a recorded demo of ML07 Transfer Learning Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:24](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/142):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#141 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/141) `open`: feat(docs): create a recorded demo of ML06 AI Supply Chain Attacks
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:24](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/141):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#140 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/140) `open`: feat(docs): create a recorded demo of ML05 Model Stealing
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:24](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/140):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#139 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/139) `open`: feat(docs): create a recorded demo of ML04 Membership Inference Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:23](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/139):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#138 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/138) `open`: feat(docs): create a recorded demo of ML03 Model Inversion Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:23](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/138):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#137 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/137) `open`: feat(docs): create a recorded demo of ML02 Data Poisoning Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:22](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/137):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)




-------------------------------------------------------------------------------

# [\#136 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/136) `open`: feat(docs): create a recorded demo of ML01 Input Manipulation Attack
**Labels**: `enhancement`, `help wanted`, `documentation/demos`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 02:17](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/136):

- [ ] Create a recorded video demo (no audio)

Video will be uploaded to [OWASP Youtube Channel](https://www.youtube.com/@owasp-mltop10)





-------------------------------------------------------------------------------

# [\#135 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/135) `open`: feat(docs): create guide for how to use Top 10 list as a Data Engineer
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:51](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/135):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#data-engineer

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:55](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/135#issuecomment-1784357453):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#134 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/134) `open`: feat(docs): create guide for how to use Top 10 list as an MLOps Engineer
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:49](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/134):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#mlops

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:55](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/134#issuecomment-1784357519):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#133 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/133) `open`: feat(docs): create guide for how to use Top 10 list as a Developer
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:47](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/133):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#developers

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:56](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/133#issuecomment-1784357594):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#132 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/132) `open`: feat(docs): create guide for how to use Top 10 list as a CISO
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:46](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/132):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#ciso

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:56](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/132#issuecomment-1784357658):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#131 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/131) `open`: feat(docs): create guide for how to use Top 10 list as a AppSec Engineer
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:43](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/131):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#pentestersecurity-engineer

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:55](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/131#issuecomment-1784357377):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#130 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/130) `open`: feat(docs): create guide for how to use Top 10 list as a ML Engineer
**Labels**: `enhancement`, `help wanted`, `documentation/guides`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-10-30 01:36](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/130):

Reference https://github.com/OWASP/www-project-machine-learning-security-top-10/blob/master/GUIDELINES.md#ml-engineeranalyst 

- [ ] Create a detailed guidelines document for how to use the information in the Top 10 list for use day to day

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-10-30 01:55](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/130#issuecomment-1784357062):

initial issue mentioned #43


-------------------------------------------------------------------------------

# [\#114 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/114) `open`: [Fortnightly] Working Group Meeting - 2023-Sep-14
**Labels**: `meeting`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-09-13 18:22](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/114):

## Current agenda

1. General project status [v0.3 - in progress](https://github.com/OWASP/www-project-machine-learning-security-top-10/milestone/3)
2. Notable PRs completed since last meeting:
  - #104 
  - #110 
3. Notable discussions:
 - #107
 - #108
 - #109
 4. Meetings:
  - WG meeting will change forward a few hours to accomodate EU morning time zones
5. Contributions and [current help wanted](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
6. Introductions (for new contributors)

## Discussions

* [Join the OWASP Slack group](https://owasp.org/slack/invite) and the [#project-mlsec-top-10 channel](https://owasp.slack.com/archives/C04PESBUWRZ)
* [Github Discussions](https://github.com/OWASP/www-project-machine-learning-security-top-10/discussions)

## Calendar Event
[Download calendar event (ICS)](https://calendar.google.com/calendar/ical/c_f818ec1e3dea1d4c80cb0f872566eccb82c5df9cc1161f3077f93eafc47889dc%40group.calendar.google.com/public/basic.ics)




-------------------------------------------------------------------------------

# [\#113 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/113) `open`: Model stealing through interaction is not mentioned
**Labels**: `issues/triage`


#### <img src="https://avatars.githubusercontent.com/u/796794?v=4" width="50">[robvanderveer](https://github.com/robvanderveer) opened issue at [2023-09-08 21:44](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/113):

The current model stealing only describes the model being stolen through parameters, but the model can also be stolen by presenting inputs, capturing the output and using those combinations to train your own model. See AI guide




-------------------------------------------------------------------------------

# [\#102 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/102) `open`: [Fortnightly] Working Group Meeting - 2023-Aug-31
**Labels**: `meeting`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-31 04:47](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/102):

## Current agenda

1. General project status [v0.3 - in progress](https://github.com/OWASP/www-project-machine-learning-security-top-10/milestone/3)
2. Contributions and [current help wanted](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
3. Introductions (for new contributors)

## Discussions

* [Join the OWASP Slack group](https://owasp.org/slack/invite) and the [#project-mlsec-top-10 channel](https://owasp.slack.com/archives/C04PESBUWRZ)
* [Github Discussions](https://github.com/OWASP/www-project-machine-learning-security-top-10/discussions)

## Calendar Event
[Download calendar event (ICS)](https://calendar.google.com/calendar/ical/c_f818ec1e3dea1d4c80cb0f872566eccb82c5df9cc1161f3077f93eafc47889dc%40group.calendar.google.com/public/basic.ics)




-------------------------------------------------------------------------------

# [\#99 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/99) `open`: feat(rendering): make PDF output from Markdown files more presentable
**Labels**: `documentation/general`, `enhancement`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-08-24 21:34](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/99):

The Top 10 list is being rendered using Markdown at https://mltop10.info

The site is being rendered using [Quarto](https://quarto.org) and the files from https://github.com/OWASP/www-project-machine-learning-security-top-10/tree/master/docs are mirrored to https://github.com/mltop10-info/mltop10.info

Currently a manual process is run for the https://github.com/mltop10-info/mltop10.info locally to render the HTML and PDF outputs which are stored in https://github.com/mltop10-info/mltop10.info/tree/main/docs and used by Github Pages.

The rendering for PDF is currently using the default method of LaTeX - example at: https://github.com/mltop10-info/mltop10.info/blob/main/docs/OWASP-Machine-Learning-Security-Top-10.pdf

Quarto has a lot of formatting options for generating PDF and this needs to be explored to make the PDF and ePUB formats look more presentable.




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

# [\#30 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/30) `open`: fix: merge existing body of work from EthicalML https://ethical.institute
**Labels**: `good first issue`, `issues/triage`


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
**Labels**: `documentation/general`, `enhancement`, `help wanted`


#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) opened issue at [2023-07-24 00:16](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/15):

Each of the Top 10 items are scored according to [OWASP's Risk Rating Methodology](https://owasp.org/www-community/OWASP_Risk_Rating_Methodology). There should be a page defining how to use the ratings to provide a severity score. This will assist practitioners in knowing 'what to fix' and 'when'.

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-08-24 21:22](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/15#issuecomment-1692428735):

- [ ] create a page showing how risk can be calculated from the top 10 list using the OWASP Risk Rating Methodology
- [ ] add information to each risk with the risk values used


-------------------------------------------------------------------------------

# [\#2 Issue](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/2) `open`: fix: merge review from @robvanderveer
**Labels**: `issues/triage`, `review needed`


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

#### <img src="https://avatars.githubusercontent.com/u/412800?v=4" width="50">[shsingh](https://github.com/shsingh) commented at [2023-09-29 00:13](https://github.com/OWASP/www-project-machine-learning-security-top-10/issues/2#issuecomment-1740146868):

>1.
>ML01
>In 'literature' the term ‘adversarial’ is often used for input manipulation attacks, but also for data poisoning, model >extraction etc. Therefore in order to avoid confusion it is probably better to rename the ML01 adversarial attack entry to >input manipulation?

addressed in : #110 

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

>8
>ML10 is called Neural net reprogramming but I guess the attack of changing parameters will work on any type of algorithm >- not just neural networks. The description also mentions changing the training data, but perhaps that is better left out to >avoid confusion with data poisoning?

addressed in: #104


-------------------------------------------------------------------------------

