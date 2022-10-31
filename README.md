# AI Psychology Starter

Code templates to get started as an AI psychologist.

Interpretability research is sometimes described as neuroscience for ML models. Neuroscience is one approach to understanding how human brains work. But empirical psychology research is another approach. I think more people should engage in the analogous activity for language models: trying to figure out how they work just by looking at their behavior, rather than trying to understand their internals. [Read more](https://www.lesswrong.com/posts/yGaw4NqRha8hgx5ny/the-case-for-becoming-a-black-box-investigator-of-language).

It was created as part of the [Language Model Hackathon](https://itch.io/jam/llm-hackathon) and several projects were submitted that you can [check out](https://alignmentjam.com/hackathon/llm#:~:text=Aarhus%20University%2C%20room%201485%2D241).

## Inspiration
-   [AI Safety Ideas project ideas](https://aisafetyideas.com/project/black-box-investigation)
-   Helpful and harmless models - Anthropic
-   Red teaming language models - Anthropic
-   OpenAI's usage examples: <https://beta.openai.com/examples/> 
-   GPT-3 products: <https://gpt3demo.com/map> 
-   [Language models are few-shot learners](https://proceedings.neurips.cc/paper/2020/file/1457c0d6bfcb4967418bfb8ac142f64a-Paper.pdf) (NeurIPS)
-   [TruthfulQA](https://arxiv.org/abs/2109.07958) - Stephanie Lin, Jacob Hilton, Owain Evans (ArXiv)
-   [Chain of thought prompting](https://arxiv.org/pdf/2201.11903.pdf) (ArXiv) 
-   [Apart Research's cognitive bias testing for the inverse scaling prize](https://github.com/apartresearch/blackbox-psych) - Esben Kran, Jonathan Rystrøm
-   [Epistemic biases in LLMs](https://forum.effectivealtruism.org/posts/sA8HC7fmYsoEABTfj/exploring-gpt3-epistemic-biases-instructgpt3-2-2) - Siméon Campos
-   Human cognitive biases in language models
-   [Artificial cognition: How experimental psychology can help generate explainable artificial intelligence](https://link.springer.com/article/10.3758/s13423-020-01825-5)
-   [Red teaming language models](https://arxiv.org/pdf/2209.07858.pdf) (really nice attacks)

# Starter code

## [R Markdown starter code](interacting-with-gpt-3.Rmd)

Contains a small test experiment along with a standardized way to get responses out of the API. See R-starter.Rmd.

## [Python notebook starter code](interacting-with-gpt-3.ipynb)

Contains the same test experiment as the R markdown starter code. See Python-starter.ipynb (this can run in the browser using Google Colab).

## [Spreadsheet GPT-3 experimental starter kit](manual-coding.xlsx)

See the template [here](https://docs.google.com/spreadsheets/d/11_6bJoU7wwHx0Nq3pySH8L91QGq3JtD8nHcNQSACax0/edit#gid=0). This is a no-code experimental kit.

## [Extract info from text](extract-info-fromt-text.ipynb)

See some ways to extract quantitative information from the text, e.g. word frequency, TF-IDF, word embeddings, and topics.

## [Inverse scaling notebook](inverse-scaling.ipynb)

From the [inverse scaling prize](https://github.com/inverse-scaling/prize). See the [instructions page](https://github.com/inverse-scaling/prize#:~:text=Submission-,guidelines,-Each%20task%20submission) for how to use it. Basically allows you to generate plots that show how the performance of the models scale with the parameter counts.

Colab to test your data for inverse scaling: <https://colab.research.google.com/drive/1IEXWy9aJaOdVKiy29LxlF-0vw9Cx-hi2>

# Data

#### Inverse scaling round 1 winning datasets

The winners of the first round winners.

<https://drive.google.com/drive/u/1/folders/1mHrPQlfB3-pfwB3iBAKheIEO3EBAb_qg> 

#### Inverse scaling

The [inverse-scaling folder](https://drive.google.com/drive/folders/1OV_HW8Sp6rWDT4EUv0n1edacoaOLqQu3) contains a lot of small datasets that can work as inspiration. E.g. biased statements, cognitive biases, sentiment analysis, and more.

<https://github.com/inverse-scaling/prize/> 

#### Harmless and Helpful language model

A large list of "chosen" and "rejected" pairs of texts. A human received two language model outputs and selected the preferred one. It's in jsonl format, so you can open it with any Python interpreter or with VScode.

[See the containing folder](https://drive.google.com/drive/u/1/folders/1W_9HPO6wElX_zT5j-DX0C31ksjYTpdbH).

<https://github.com/anthropics/hh-rlhf> 

#### Red teaming dataset

Contains a lot of humans' attempts at tripping up a language model and getting it to answer in harmful ways.

[red_team_attempts.jsonl](https://drive.google.com/drive/u/1/folders/18orPwvn48c75I9A7dp_37bgu2QTUmGRn)

<https://github.com/anthropics/hh-rlhf> 

#### TruthfulQA

This repository contains code for evaluating model performance on the TruthfulQA benchmark. The full set of benchmark questions and reference answers is contained in TruthfulQA.csv. The paper introducing the benchmark can be found [here](https://arxiv.org/abs/2109.07958).

<https://github.com/sylinrl/TruthfulQA/blob/main/data/v0/TruthfulQA.csv>

#### MathQA

This is the official repo for the ACL-2022 paper "[Learning to Reason Deductively: Math Word Problem Solving as Complex Relation Extraction](https://arxiv.org/abs/2203.10316)". Text describes free-form world states for elementary school math problems.

<https://github.com/allanj/deductive-mwp>

#### Language models are few-shot learners

You can train language models with training examples in its prompt.

Data: <https://github.com/openai/gpt-3/tree/master/data>

<https://github.com/openai/gpt-3>

#### Moral Uncertainty

We provide a dataset containing a mix of clear-cut (wrong or not-wrong) and morally ambiguous scenarios where a first-person character describes actions they took in some setting. The scenarios are often long (usually multiple paragraphs, up to 2,000 words) and involve complex social dynamics. Each scenario has a label which indicates whether, according to commonsense moral judgments, the first-person character should not have taken that action.

Our dataset was collected from a website where posters describe a scenario and users vote on whether the poster was in the wrong. Clear-cut scenarios are ones where voter agreement rate is 95% or more, while ambiguous scenarios had 50% ± 10% agreement. All scenarios have at least 100 total votes.

<https://github.com/JunShern/moral-uncertainty#dataset>

<https://moraluncertainty.mlsafety.org/> 

#### IMDB dataset

This dataset contains a lot of movie reviews and their associated rating. It is classically used to train sentiment analysis models but maybe you can find something fun to do with it!

[See containing folder](https://drive.google.com/drive/folders/18orPwvn48c75I9A7dp_37bgu2QTUmGRn).
