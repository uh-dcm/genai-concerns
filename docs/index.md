---
hide:
  - navigation
---

# Concerns on the use of generative AI in social science research

## Background
Overall, there has been quite a bit of interest on the use of generative AI (genAI) in social science for data generation and analysis. For example, to summarise this discussion and highlight ongoing work, Chris Bail published an article [‘Can Generative AI improve social science?’](https://www.pnas.org/doi/full/10.1073/pnas.2314021121) in May 2024, summarising current debate on both the benefits and concerns related to using generative AI for social science research and arguing that genAI has great potential in these fields. At the same time, some social scientists have felt less optimistic about these opportunities.

In hopes to develop practices in social sciences, this document is intended to become a repository which outlines concerns and issues to address and engages them with more critical research. 

We assume our readers are familiar with terms like ‘generative AI’, ‘large language models’, ‘Foundation Models’. If not, Bail’s article provides a useful summary of these. 

### How to contribute!
We would welcome any suggestions for additions to this list!

1. (Our preference!) Make a pull request for this [repository](https://github.com/uh-dcm/genai-concerns/)!
2. Contact us via email: <matti.nelimarkka@helsinki.fi> and <adeline.clarke@helsinki.fi> 

## General limitations
Overall, there are general concerns related to the application of large language models across all application areas.
These are highlighted e.g. in Bail’s article as concerns, but even while these are acknowledged as issues, there is much less know-how on how to correctly address these issues.

###  Reproducibility

Replicability of research using generative AI is of concern due to the probabilistic nature of the models.
‘Temperature’ parameters can be used to combat this but there isn’t consensus on what these should be set to and they come with drawbacks of repetition that may be problematic in some research settings.
Another issue is that as the models change and develop, their outputs will as well, making it difficult to reproduce results at a later date.
Finally, results may be dependent on which generative AI was used within the research. 

* [Bisbee et al.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/B92267DC26195C7F36E63EA04A47D2FE/S1047198724000056a.pdf/synthetic-replacements-for-human-survey-data-the-perils-of-large-language-models.pdf) found that between April and July 2023, changes in the algorithm in ChatGPT 3.5 Turbo would have significantly changed their results. 

### Bias

Generative AI tools exhibit the human biases found in their training materials.
Bail argues prompt engineering shows some promise in addressing this and these biases may be easier to remove from generative AI than human populations, but this requires researchers being able to identify the bias and is hindered by researchers having little access to material used to train the model.
This bias can be seen as a ‘bug’ or a ‘feature’ and may be useful in some research applications.
We also don’t know what the developers have done to limit or prevent certain biases (such as racism) through fine-tuning to safeguard against their generative AI producing unappealing or toxic content. 

* See Boelaert et al. “Machine Bias”, discussed [below](https://osf.io/preprints/socarxiv/r2pnb).
* Santurkar et al. ask [‘Whose Opinions Do Language Models Reflect?’](https://arxiv.org/abs/2303.17548), quantifying results gained from using LLMs in comparison to opinion polls. Even when prompted to represent a certain US demographic group, the overall results tend to reflect more liberal, younger and educated respondents rather than the general population.
* Similarly, [Atari et al.](https://osf.io/preprints/psyarxiv/5b26t) show that LLMs best reflect WEIRD (Western Educated Industrialised Rich Democratic) societies.
* [Pellert et al.](https://journals.sagepub.com/doi/epub/10.1177/17456916231214460) consider the psychometric profile of LLMs, concluding that LLMs portray traits of extraversion and agreeableness, and don’t show neuroticism.  
* [Chen et al.](https://www.pnas.org/doi/epub/10.1073/pnas.2316205120) show that GPT produces results that are more rational, and homogenous than humans. 
* [Nelimarkka](https://osf.io/preprints/socarxiv/fkj63) fine-tuned an LLM to have a marxist viewpoint. In doing so, he demonstrated that the base model itself is not neutral and has a ‘viewpoint’.
* [Addulhai et al.](https://arxiv.org/pdf/2310.15337) use a psychological assessment tool (Moral foundations theory) to assess typical responses by LLMs and find that LLMs have a bias towards reflecting politically conservative people. In their paper they also highlight a number of risks coming from their use.
* [Ashwin et al.](https://journals.sagepub.com/doi/full/10.1177/00491241251338246) compare using LLMs with expert coding for analysis of open-ended interviews with a large number of participants (in their case, interviews with Rohinga refugees and their hosts in Bangladesh) and find that LLMs have are biased and that the resultant prediction errors are not random. They suggest it is 'preferable to train a bespoke model on a subset of transcripts coded by trained sociologists rather than use an LLM'.
* [Qu and Wang](https://www.nature.com/articles/s41599-024-03609-x) also find that ChatGPT has better performance for WEIRD countries (and best performance for the USA) and demonstrate other biases around gender, ethnicity, age, education, social class. They use data World Values Survey to evaluate the LLM's performance at producing silicon samples and highlight 3 challenges to address before LLMs can be used in the social sciences: 'global applicability and reliability', 'demographic biases', and 'complexity and choice variability in LLM simulations'.

### Ethics

The ethical concerns with the use of generative AI in research include: whether consent should be sought before including generative AI in experiments involving human subjects, generative AI producing harmful content or misinformation when interacting with human subjects (especially if interactions are not closely ‘supervised’, although arguably generative AI could allow researchers more control over content than having two humans interacting), concerns with storage of identifiable, private or confidential data if private corporations control generative AI tools used in research, and environmental impact (see below). The ethical advantages include: generative AI being used to simulate dangerous scenarios and using generative AI to diagnose ethical issues.

* Weidinger et al. provide a [“Taxonomy of risks posed by language models”](https://dl.acm.org/doi/pdf/10.1145/3531146.3533088) covering 21 ethical and social risks covering areas of: ‘Discrimination, Hate speech and Exclusion’, ‘Information Hazards’, ‘Misinformation Harms’, ‘Malicious Uses’, ‘Human-Computer Interaction Harms’, and ‘Environmental and Socioeconomic Harms. 
* Another concern, highlighted by [Pasquale and Sun](https://virginialawreview.org/articles/consent-and-compensation-resolving-generative-ais-copyright-crisis/), is whether creators have consented to, or been compensated for their work being used to train genAI tools. 
* In [AI Snake Oil](https://www.aisnakeoil.com/), Narayanan and Kapoor demonstrate that training generative AI tools comes at a human cost, highlighting that annotators which are used in many tasks such as labelling possible toxic output, are often overworked and underpaid. 
* There are dangers from conversations between genAI chatbots and vulnerable people. In a tragic [example](https://www.euronews.com/next/2023/03/31/man-ends-his-life-after-an-ai-chatbot-encouraged-him-to-sacrifice-himself-to-stop-climate-), a Belgian man died by suicide after engaging with an AI chatbot who encouraged him to sacrifice himself to help the climate crisis. This is not the only example. In both these cases show the dangers of emotional attachments these individuals felt with the chatbots. While some genAI tools are trained NOT to suggest they’re capable of feeling human emotions, these recent examples show that further regulation is likely required. 
* Another real-world [example](https://www.boston.com/news/the-boston-globe/2023/07/21/mit-student-ai-racial-blind-spots/) of the ethics of these tools comes from the racial changes suggested to a computer scientist’s profile image when she asked for a photo to be adapted to look ‘more professional’ for use of LinkedIn and her Asian features were replaced with lighter skin and blue eyes. 

### Hallucination/ Junk Science

Generative AI can often create inaccurate information with high confidence.
This is partly due to the models being trained on datasets which can contain misinformation or flawed content.
In some cases, hallucinations have also become defamatory: In 2025, a Norwegian man [filed a complaint](https://techcrunch.com/2025/03/19/chatgpt-hit-with-privacy-complaint-over-defamatory-hallucinations/) after ChatGPT falsely claimed he had been convicted of murdering two of his children.
As such incorrect personal data points are difficult or impossible to correct by such services, they are, in effect, breaching the GDPR.

[Mervaala and Kousa](https://jdmdh.episciences.org/15304) have addressed such issues regarding the limitations of ChatGPT’s context window: for example, when the amount of text an LLM can analyse is exceeded, the model may concoct the rest of the analysis based on the beginning of the document.

### Environmental Impact

The environmental cost of training and using generative AI tools are significant and as these tools become bigger (and better) so will their footprint! 

## Application areas

### Automated Text Analysis 
- **Claim:** Generative AI shows promise within text analysis and could be used for content analysis (such as classification, credibility assessment, topic identification) with accuracy that surpasses that of Amazon Mechanical Turk. It is not yet superior to expert coding, but has comparative advantages including unlimited attention-span, consistency, speed, and objectivity. 
- **Counterclaim:** [Ollion et al.](https://osf.io/preprints/socarxiv/x58kn) conducted a literature review and found mixed results from few- and zero-shot text annotation by ChatGPT “and kin models”. Overall results showed ChatGPT was generally outperformed by models fine-tuned on human annotations but may perform better than crowdsourced annotation. While different studies demonstrated varied performance by the LLMs, generally recall was better than precision (more false positives than false negatives). One issue raised in the review was that different studies used different metrics to evaluate ChatGPT. Other concerns raised by the authors were reproducibility of research using ChatGPT for annotation, privacy and copyright considerations, and further dominance of English language in research. 

### Synthetic Survey
- **Claim:** Generative AI could be used to create ‘silicon samples’ after provision of a number of background variables and traits of respondents, thus allowing a representative sample to be used where ‘convenience samples’ are otherwise used for practical reasons. These synthetic surveys would also be able to be longer and include more invasive questioning.
    - A good example of these synthetic surveys is [this](https://www.cambridge.org/core/journals/political-analysis/article/abs/out-of-one-many-using-language-models-to-simulate-human-samples/035D7C8A55B237942FB6DBAD7CAA4E49) article which used GPT-3 'conditioned' using real survey data (such as ANES) to avoid unwanted algorithmic bias, and instead to produce responses that correspond to specific demographics.
- **Counterclaims:**
    - [Boelaert et al.](https://osf.io/preprints/socarxiv/r2pnb) caution against the use of silicon samples, particularly in opinion polling . In their experiment, these samples display random bias for each question which they term “Machine Bias”. Their experiment, which compares Llama, Mixtral and GPT-4, and attempts to use LLMs to replicate results of the World Values survey from Australia, Mexico, Germany, Russia and the US, shows that LLMs are bad at predicting attitudes, show no systematic social bias (ie. the bias doesn’t correlate with a specific social group) and low adaptability to input of sociodemographic properties to display. 
    - UX consultancy [NNg](https://www.nngroup.com/articles/synthetic-users/) argue that a better use case for synthetic survey participants is to ‘supplement’, not ‘substitute’ (such as in hypothesis identification or desktop research) as their responses tend to be ‘shallow or overly favourable’.  
    - [Bisbee et al.](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/B92267DC26195C7F36E63EA04A47D2FE/S1047198724000056a.pdf/synthetic-replacements-for-human-survey-data-the-perils-of-large-language-models.pdf) used ChatGPT 3.5 Turbo to create silicon samples based on real respondents from the ANES with questions similar to those in the ANES. They considered the mean and variance of responses along with correlation between persona characteristics and responses, and sensitivity to changes in the prompts. They found that their results were not replicable (they showed significant differences due to underlying algorithm changes between April and July 2023). While every synthetic mean was within 1 standard deviation of ANES results, the synthetic data show less variance and differences in distributions would have led to different inferences from the synthetic data. 
    - [Dentella et al.](https://www.pnas.org/doi/epdf/10.1073/pnas.2309583120) investigated the claim that LLMs have a ‘human-like language understanding’ by testing LLM ability to learn linguistic phenomena and  comparing human and LLM performance in determining whether sentences were grammatical or not. While not a ‘synthetic sample’, their results have impacts for use of LLMs in survey research by demonstrating a bias towards ‘yes’ in yes-no questions by LLMs as well as instability in LLM responses.   
    - [Dentella et al.](https://www.pnas.org/doi/epdf/10.1073/pnas.2309583120) also found a ‘yes’ bias from LLMs and that there is instability in their responses, contradicting the claim that LLMs possess ‘human-like’ language ability.. This study found that LLMs were unable to produce ‘stable and accurate answers, when asked whether a string of words complies with or deviates from their next-word predictions’ which is an area humans are ‘universally good’ at. Thus, they show that LLMs cannot currently be used to understand natural language. 
    - [Santurker et al.](https://arxiv.org/pdf/2303.17548) show that LLMs are particularly bad at representing some demographic subgroups such as over-65s, Mormons and the widowed. This study looks at US demographic groups; it is likely these issues extend outside of a US context.
    - [Von der Hayder et al.](https://arxiv.org/pdf/2407.08563) considered whether LLMs could be used to estimate vote choice in Germany by generating a silicon sample based on the 2017 German Longitudinal Election Study. They found that vote choice was not predicted accurately and results indicated a bias towards left-wing parties. Additionally, their results indicated that the LLMs were unable to demonstrate nuances in voting behaviours beyond ‘typical’ voter types. 
    - [Ramezani and Xu](https://arxiv.org/pdf/2306.01857) study whether English-language LLMs ‘understand’ moral norms in various countries using the World Values Survey and PEW global surveys. They find that these are more accurately inferred for Western contexts and show that this can be improved through fine-tuning at the expense of their ability to estimate moral norms in English-speaking contexts.  
    - [Durmas et al.](https://arxiv.org/pdf/2306.16388) consider responses generated by LLMs and find that these resemble most closely respondents from the USA, Canada, Australia and some European and South American countries. When prompted to represent another country, the responses often contained ‘harmful cultural stereotypes’. Additionally, their study shows the distribution of responses to questions often differs greatly from that of human respondents as the LLM shows a high confidence in a single response where humans have more diverse viewpoints.
    - [Lyman et al](https://journals.sagepub.com/doi/10.1177/00491241251342008) caution about the importance of model choice, acknowledging that there are a rapidly changing set of choices. They acknowledge that without "social science-specific guidance", it can be difficult to make an informed choice and offer a "clear process" to ensure a good choice is made.
      
- **Claim:** Generative AI could be used to create ‘silicon samples’ _when_ the above-mentioned issues on representation are addressed.
- **Counterclaim:**
    - [Boelaert et al.](https://doi.org/10.1177/00491241251330582) show that the models seem to have effects which cannot be explained just through lack of representativeness, and rather highlight more fundamental issues with the operation of LLM.

### Synthetic Experiments
- **Claim:** Generative AI has successfully reproduced some experiments (such as the Milgram experiment) and reflect known phenomena (such as the Prisoner’s Dilemma), there is an opportunity for generative AI to reproduce experiments. He also highlights a study which found a correlation of 0.86 between the results of 482 studies and synthetic experiments using GPT-4 indicating this opportunity could be widespread. 
- **Counterclaim:** The positive findings about the replication of the Milgram Experiment listed above comes from [Aher et al.](https://arxiv.org/pdf/2208.10264) who also were able to replicate the results of the Ultimatum Game and Garden Path Sentences. However, genAI could not replicate the ‘Wisdom of Crowds’ which shows that not all known human behaviour phenomena will be reflected in genAI output, and is a cautionary case against using genAI for their discovery. 

### Generative Agent-Based Models
- **Claim:** generative AI can be used to simulate populations which could lead to better, richer, ABMs thus enabling deeper research.  
- Currently no counter claims!

### Blending Simulation and Human Experiment

- **Claim:** There are a number of articles which demonstrate that LLMs are capable of convincingly impersonating humans. Bail highlights this as an opportunity for content creation (eg. production of text designed to elicit a specific response in human subjects or creation of two similar images depicting different races). Bail also believes generative AI provides an opportunity to create chatbots that are convincingly human, to include AI participants with particular traits within research on groups and influence.
- [Cheng et al.](https://arxiv.org/abs/2305.18189) look at stereotypes that are found in LLM output and present a method called 'Marked Personas' which measures these. This method first prompts the LLMs to generate personas, and then identified words which distinguish groups. THey find higher rates of racial stereotypes in LLM output (compared with human-written personas from the same prompts) and evidence of 'othering and exoticising' non-white, non-male groups. 





