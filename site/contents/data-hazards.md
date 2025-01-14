# Data Hazard labels

[//]: # (TODO: Link to contribution guidelines)

This page contains the Data Hazard labels themselves.
These labels, descriptions, examples, and safety precautions will evolve as we develop the hazard labels with the communities who will use them.
We welcome you to suggest changes via [email](mailto:grp-ethicaldatascience@groups.bristol.ac.uk) or [GitHub](https://github.com/very-good-science/data-hazards).

Each hazard has:
- __Hazard__ image, title, and description which represents and describes the risk.
- __Examples__ to clarify what the hazard covers.
- __Safety Precautions__ - things that we would want to see done **before** the research is deployed.

They are designed to help us think about the different types of hazards

[//]: # (TODO: Add 2 examples for each hazard - with a link if possible)
[//]: # (TODO: Add safety precautions for each hazard - with a link if possible.)

````{panels}
:container: container-fluid
:column: col-6 p-3
:img-top-cls: p-3 bg-warning
:header: bg-warning
:body: bg-warning 
:footer: bg-warning 

:img-top: /images/hazards/general-hazard.png

__Hazard: Data Hazard__

Data Science is being used in this output, and any negative outcome of using this work are not the fault of "the algorithm" or "the software". 

This hazard applies to __all__ Data Science research outputs.

^^^

All other Data Hazard examples could feature as examples here.

+++
__Safety Precautions:__
-  Users of this work should be informed that __the repsonsibility for using this work responsibly and ethically, lies with each person who impliments it in a project or product.__

---
:img-top: /images/hazards/reinforce-bias.png

__Hazard: Reinforces existing biases__

Reinforces unfair treatment of individuals and groups. This may be due to for example input data, algorithm or software design choices, or society at large. 

__Note:__ this is a hazard in it's own right, even if it isn't then used to harm people directly, due to e.g. reinforcing stereotypes.

^^^

__Example 1__: [Natural Language Processing tools can reinforce sexist tropes about women](https://arxiv.org/abs/1607.06520). 

__Example 2:__ [Automated soap dispensers that do not work for black people](https://metro.co.uk/2017/07/13/racist-soap-dispensers-dont-work-for-black-people-6775909/)

+++
__Safety Precautions:__
- Test the effect of the algorithm for different marginalised groups, considering different definitions of [bias]() and [fairness]().
- Think about the input data, what intrinsic bias it contains, and how this can be reduced (for example by having a more representative data set).
- Think about the bias of the algorithm, what intrinsic bias it contains, and how this can be reduced.


---
:img-top: /images/hazards/classifies-people.png

__Hazard: Ranks or classifies people:__
 
Ranking and classifications of people are hazards in their own right and should be handled with care.

To see why, we can think about what happens when the ranking/classification is inaccurate, when people disagree with how they are ranked/classified, as well as who the ranking/classification is and is not working for, how it can be gamed, and what it is used to justify or explain.

^^^

__Example 1:__ [Facial recognition categorising human images by sexual orientation](https://www.bbc.co.uk/news/technology-41188560). 

__Example 2:__ [School league tables](https://www.bristol.ac.uk/media-library/sites/cmm/migrated/documents/limitations-of-league-tables.pdf) (which rank the perfmance of schools).

+++
__Safety Precautions:__
- Test the effect of the algorithm or technology for different marginalised groups. 
- Carefully consider the validity of any classification groups and work with subject specialists from the application area on this. 
- Be transparent about what the weaknesses of the algorithm and technology are: test how can it be fooled. 
- Consider alternatives to ranking/classification, for example treating people equally, increasing resources for the issue at hand, or allowing people to self-select.

---
:img-top: /images/hazards/environment.png

__Hazard: High Environmental Cost__

This hazard is appropriate where methodologies are energy-hungry, data-hungry (requiring more and more computation), or require special hardware that require rare materials. 

^^^

__Example 1:__ Cryptocurrency requires [vast energy usage](https://www.bbc.co.uk/news/technology-56012952)

__Example 2:__ Language models [require larger and larger datasets](http://faculty.washington.edu/ebender/papers/Stochastic_Parrots.pdf)

+++
__Safety Precautions:__
- Consider in what circumstances it is worthwhile to use this type of methodology.
- Consider future work that would reduce the need to use increasingly more resources.

---
:img-top: /images/hazards/lacks-community.png

__Hazard: Lacks community involvement__
This applies when technology is being produced without input from the community it is supposed to serve.

^^^

__Example 1:__ Research into cures for Autism generally ([which are not wanted by Austistic people](https://www.theguardian.com/commentisfree/2009/jan/14/autism-health)).

__Example 2:__ Samaritan's Radar app highlighted people who may be struggling to cope on Twitter, and was [withdrawn following wide criticism](https://www.samaritans.org/about-samaritans/research-policy/internet-suicide/samaritans-radar/). 

__Example 3:__ [Algorithmic colonisation of Africa](https://script-ed.org/article/algorithmic-colonization-of-africa/)

+++
__Safety Precautions:__
- Ask the people who the works is about if they want this kind of solution, and co-create or [co-produce](https://www.youtube.com/watch?v=6XF0GFDYw3E) research with them as partners.
- Test the effectiveness of the algorithm or technology for different marginalised groups.
- Consideration of issues of power, consent and trust. 


---
:img-top: /images/hazards/misuse.png

__Hazard: Danger of misuse__
There is a danger of misusing the algorithm, technology, or data collected as part of this work.

^^^

__Example 1:__ Statistical method to do impossible tasks, for example [predicting future human behaviour]().

__Example 2:__ The collection of a large data set of individuals, which could be hacked, or used for other purposes.

+++
__Safety Precautions:__
- Write clear instructions about in what circumstances the algorithm/technology will work or give valid answers and present these wherever the work is presented.
- If work is piloted outside of this context, it must be re-tested.
- Follow data governance guidelines.

---
:img-top: /images/hazards/difficult-to-understand.png

__Hazard: Difficult to understand__
There is a danger that the technology is difficult to understand. 
This could be because of the technology itself is hard to interpret (e.g. neural nets), or problems with it's implementation (i.e. code is not provided, or not documented).

Depending on the circumstances of its use, this could mean that incorrect results are hard to identify, or that the technology is inaccessible to people (difficult to implement or use).

^^^

__Example 1:__ Deep learning is used to perform [credit-scoring](https://www.moodysanalytics.com/risk-perspectives-magazine/managing-disruption/spotlight/machine-learning-challenges-lessons-and-opportunities-in-credit-risk-modeling) (i.e. could deny people credit), but it is difficult to understand (and therefore check) what these decisions are based on.

__Example 2:__ Even when journals have a policy of having code and data availability, published researchers can be unaware of what they agreed to and resist sharing it, as [this](https://www.pnas.org/content/115/11/2584) paper surveying Science publications shows.

+++
__Safety Precautions:__
- Make research code Open Source with [an appropriate software license](https://choosealicense.com/) where possible. Your local [Research Software Engineering](https://society-rse.org/) group may be able to help you with this.
- Compare results to white box (explainable) methods such as [Random Forest](https://en.wikipedia.org/wiki/Random_forest) or [Regression](https://en.wikipedia.org/wiki/Regression_analysis), which may perform just as well. 

---
:img-top: /images/hazards/direct-harm.png

__Hazard: May cause direct harm__
The application area of this technology means that it is capable of causing direct physical or psychological harm to someone even if used correctly e.g. healthcare and driverless vehicles may be expected to directly harm someone unless they have 100% accuracy.

^^^

__Example 1:__ Software running on driverless cars can fail, allowing the car to crash, which can injure or [kill](https://www.nytimes.com/2021/04/18/business/tesla-fatal-crash-texas.html) [people](https://www.bbc.co.uk/news/technology-54175359).

__Example 2:__ AI chatbots, which are becoming more widely used in the medical field, may be used as medication reminders or for triaging services based on need. 

+++
__Safety Precautions:__
- It is even more important that work of this nature is well-tested and that any "bugs" (mistakes in software) are found.  
- Carefully consider acceptable (and likely) margins of error - if no error is acceptable in this use case, then should it be done at all? 


---
:img-top: /images/hazards/privacy.png

__Hazard: Privacy__
This technology may risk the privacy of individuals whose data is processed by it. 

^^^

__Example 1:__ Facial recognition technologies are a [widely recognised risk to privacy](https://www.nature.com/articles/d41586-020-03187-3). 

__Example 2:__ Apps designed to monitor children's digital activity risk children's privacy, and can be repurposed maliciously as stalkerware.

+++
__Safety Precautions:__

- Ensure there is explicit and well-informed consent from any participants. 
- Carefully consider the digital and cyber security of data and future inferences.

---
:img-top: /images/hazards/automates-decision-making.png

__Hazard: Automates decision making__
Automated decision making can be hazardous for a number of reasons, and these will be highly dependent on the field in which it is being applied. 
We should ask ourselves whose decisions are being automated, what automation can bring to the process, and who is benefitted/harmed from this automation. 

^^^

__Example 1:__ [Predictive policing](https://www.brennancenter.org/our-work/research-reports/predictive-policing-explained) is used to decide where to deploy officers.

__Example 2:__ Credit scores are produced automatically and rarely involve human input. 

+++
__Safety Precautions:__
- Inclusion of feedback into the system, so that poor or incorrect decisions are not repeated.
- Rigorous testing across a broad range of scenarios, and edge cases. This should include those with experience of the domain, and those about whom decisions are being made.
- Consider human-in-the-loop solutions for higher risk decisions. 
- Ensure outputs of decision making processes are interpretable. 

---
:img-top: /images/hazards/lacks-informed-consent.png

__Hazard: Lacks Informed Consent__
This hazard applies to datasets or algorithms that use data which has not been provided with the explicit consent of the data owner/creator. This data often lacks
other contextual information which can also make it difficult to understand how the dataset may be biased.

^^^

__Example 1:__ Large public social media datasets rarely collect informed consent from 'participants'. 

__Example 2:__ [Data linkage projects](https://bmcmedethics.biomedcentral.com/articles/10.1186/s12910-015-0070-4) tend not to involve informed consent. 

+++
__Safety Precautions:__
- Being clear about the limitations of any ground truth inferences made from the data.
- Systems built solely with this type of data should not be applied in practice. 

````

