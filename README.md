# Trying To Tap Large Language Models' Vast Potential In Knowledge Generation 

![alt text](images/header.webp)

## Why I'm working on this passion project

*By: Daniel Rosehill*
*Oct 31st 2024*

Since the early summer of 2024, I've been working on a system (for personal use) for creating an optimised workflow for generating and organising knowledge "derived" from AI tools. 

To many, the idea of describing the outputs of AI as "knowledge" seems paradoxical or even laughable. My perspective is different and like all instances in which my thinking differs from convention, I feel more encouraged to share it, if for no other reason than to widen the pool of perspectives on this important topic. 

Here's the gist of my counter-argument to AI and LLM skeptics:

### 'Knowledge' is a subjective concept

*All* information, whether it's derived from humans or computers, can be treated as suspicious. 

One man's knowledge is another's wild conspiracy theory - and another's unvalidated opinion. We each curate what we regard to be our own collection of "knowledge" and we each own our own version of truth. Like fingerprints, none are identical. To suggest that LLMs are rupturing a pristine and objective set of thinking, is firstly, mistaken.

We may be able to point to objective flaws in the types of information that large language models (LLMs) generate. Things like hallucinations and shallow context depths are understood and widely-discussed challenges. These are also challenges that are actively being explored and mitigated by technologies like RAG.

However, to dismiss the utility of robust LLMs in helping to mine and explore human understanding is like saying that  we should stop funding public libraries because some of the books they contain are evidently hogwash or contain old science that has since been proven to be baseless. Or that we should abandon using search engines like Google because much of the information they retrieve is non-useful and inaccurate affiliate marketing. 

My heartfelt belief is that everyone who champions freedom of expression of believes in the wonderful potential that arises when informations collaborate on sharing ideas should celebrate the advent of LLMs. If growing up through the advent of dial-up internet and working in the knowledge economy qualifies me to call myself a "digital native," I think LLMs are the greatest advent for digital natives since powerful computing and connectivity both became ubiquitous. 

My interest in exploring how humans and LLMs can *collaborate* in mapping knowledge emanates from these foundational beliefs. 

Inspired by the workings of the human mind, LLMs offer - to anybody who can pay a subscription to one or host one - an incredibly powerful mechanism for retrieving and synthesising information. 

This does not mean that LLMs are immune from things like censorship and manipulation that reflect not technical challenges but the intention of humans. They are not. And I argue that the justifiable concern about AI ethics has led to mainstream LLMs both being overly censored and reflecting a specific cultural bias that fails to understand regional variation in culture. Although grounded in noble attempts to prevent LLMs from causing harm, I think that these are mistakes.

But to point solely to the deficiencies of any emerging technology is to miss the huge opportunity they can bring in knowledge retrieval. And knowledge retrieval is arguably the order of the day. Being saturated in data is arguably just as useless as being deficient in it. Traditional search engines which rely on indexing emerging data struggle. LLMs present a very different and powerful new approach that is - at least - a worthy accompaniament to existing search tools. 

###  Why capture and organise LLM outputs in the first place, though?

The modest knowledge-base project I am working on as a passion project "built in public" is simply an attempt to come up with a technical system that can play to the strengths of both AI tools and humans by providing a digitally robust system for capturing and mapping the various fundamental components of the LLM chains in use today (my definition of these is something like: prompts, outputs, model and agent configurations, and contextual data - the latter includes vectorised knowledge stores and RAG systems). 

My focus since I began working on this has been on capturing LLM outputs at scale - and I began building this solely because output capture has been neglected in virtually all major LLMs. Like many passion projects, it began from with failing to find a solution among current technologies that seemed to fit intuitively with my needs. 

The relative paucity of tools to store LLM outputs felt - and to me still does - like an enormous pity. 

Capturing text digitally in the year 2024 is trivially easy: millions of outputs can be stored in a markdown archive that barely touches 100 MB. Tools for taking notes, reading notes, and mapping connections as graphs also abound.

Although no real technical constraints prevent them from doing so, mainstream LLM platforms (ChatGPT, Claude, et al) have paid almost no attention to facilitating functional systems that allow users to retain and organise the data they receive back from LLMs (collectively, outputs).

My motivations for developing my own system for doing precisely this were two-fold:

- Firstly, to enable the use of LLM outputs as a sort of "first entry" notepad to elucidate directions for further research and enquiry. Given the digital "cheapness" of text storage mentioned earlier, I felt that being digital selective in storage was not worth the time which such filtering would take. 
  
- Secondly to develop my own knowedge repository, albeit one derived from AI. As human-authored components of the LLM chain, I believe that it makes sense to capture prompts and outputs separately and that both provide independent value as data sources. Prompts provide an imprint of the users' questions and thoughts while outputs provide the raw data supplied back by LLMs. 

The simple use-case I've facilitated is having a personal notepad/wiki (which is far from revolutionary or imaginative!). But unlike a human-authored notepad, this has scaled at a pace that's rather quicker (some of my notes are saved at danielgoesprompting.com)! My enthusiasm for both exploring LLM use-cases and learning in general have facilitated quite a quick expansion. 

As my personal AI-derived "vault" has scaled into the thousands, I've chanced upon a secondary benefit of storing LLM outputs at scale that takes the project in more imaginative directions: 

AI derived knowledge vaults quickly become unwieldly and do not jive well with traditional organisation systems. Systems that require users to manually establish connections between nodes to visualise knowledge on a graph are suitable for small use-cases but quickly become impractical with scale. 

But as much as this presents a challenge, I believe it presents an opportunity. 

If the main benefit of using LLMs is to assist with finding "directions" in research avenues rather than retrieving 100% accurate information, keeping track of those directions - the relationships between prompts, outputs, and follow up conversations - is arguably much more interesting and valuable than the knowledge at face value. Or at least, they both offer independent utility.

![alt text](images/image2.webp)

## Secondary Benefits That Derive From Organised Prompt And Output Storage In Information Systems

With that in mind, as my project has evolved, I've begun thinking about a few specific additional directions:

- How an AI middleware layer could be used to autonomously establish the relationships between stored outputs, helping users to make sense of the growing collection of AI-generated knowledge as it grows. Practical use-cases in a collaborative knowledge-sharing environment might be allowing users to discover existing lines of enquiry into overlapping topics that have been conducted within the organisation, potentially allowing for collaborations that mightn't have otherwise occurred.
- Topic clustering can help make sense of the evolution of the individual or organisation's research as it evolves, reshapes, and grows. This can be visualised. 
- "AI on top of AI". It's becoming increasingly common for KMs and wikis to offer "AI on top of AI". Systems like RAG can use the AI-generated knowledge repository as a basis for mining previously retrieved information. This can take the form of interactive chatbots which are trained on the knowledge repository for enhanced discovery. 
-  LLMs are fast evolving. By collecting outputs, one builds up a repository of data that could later be mined to determine insights about the evolution of LLM models themselves. Once prompts and outputs are properly related and saved in this system, this data could be used to determine how LLM response patterns are shifting over time; which use-cases are becoming more feasible as capabilities evolve; and which prompting strategies need refining and adjustments. 

These and many other features can be enabled by robust output management and storage. 
 

## Author

Daniel Rosehill  
(public at danielrosehill dot com)

## Licensing

This repository is licensed under CC-BY-4.0 (Attribution 4.0 International) 
[License](https://creativecommons.org/licenses/by/4.0/)

### Summary of the License
The Creative Commons Attribution 4.0 International (CC BY 4.0) license allows others to:
- **Share**: Copy and redistribute the material in any medium or format.
- **Adapt**: Remix, transform, and build upon the material for any purpose, even commercially.

The licensor cannot revoke these freedoms as long as you follow the license terms.

#### License Terms
- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **No additional restrictions**: You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

For the full legal code, please visit the [Creative Commons website](https://creativecommons.org/licenses/by/4.0/legalcode).