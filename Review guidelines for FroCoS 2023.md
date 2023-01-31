﻿# Review guidelines for FroCoS 2023 

This guidance document is a minimally modified version of the one for ISWC 2022 (thanks to [Aidan Hogan](https://aidanhogan.com/)!) which, in turn was heavily inspired by similar guidelines provided for SIGMOD. The goal is to ensure the quality of  the overall reviewing process of FroCoS  for the benefit of our research community. The first section offers some general guidance relating to the content of reviews. The second section offers a suggested structure for reviews.


## Table of Contents                                                                

- [Review content](#ReviewContent)
- &nbsp;&nbsp;&nbsp;&nbsp; [Provide a detailed and constructive review](#ProvideD&CReview)
- &nbsp;&nbsp;&nbsp;&nbsp;  [Be civil and polite](#BeCivilAndPolite)
- &nbsp;&nbsp;&nbsp;&nbsp; [Adequately justify your recommendation](#AdequatelyJYRecomm)
- &nbsp;&nbsp;&nbsp;&nbsp; [Be honest about your understanding of the paper](#BeHonestAYUnderstandingOfThePaper)
- [Suggested review structure](#SuggestedRevStructure)
                                
## Review content  {#ReviewContent}

We discuss four guidelines for reviews. We include examples of things to avoid in reviews, compared with examples of what would be better to include in a review.
                                                
### Provide a detailed and constructive review  {#ProvideDAndCReview}

Please provide reviews that help the authors to improve their work, particularly in cases where your recommendation is to reject the paper. Please avoid vague, subjective or overly-general feedback that could apply to any paper. Rather aim to provide detailed feedback that is specific to the paper under review, and indicates concrete ways in which the paper could be improved.

| Examples to avoid |	Better examples |
|----------- |----------- | 
| “The paper lacks novelty.”
(No justification or details provided.) <br><br>| “The key method described in Algorithm 1 appears to be very similar to that of Doe et al. [A], with only minor changes to the recursive aspect. The authors should clarify the novelty or relation of their method with respect to that proposed by Doe et al.” |
| 	“The techniques seem trivial.”
 <br><br>
(No justification or details provided.)|“The proof of the key result, described in Theorem 1, involves a standard reduction from an existing result that is described, for example, in Section 4.2 of the textbook by Zoe [A].” |
|	“The paper is poorly written” <br><br>
(No justification or details provided.) |
	“I found the paper difficult to follow; for example:  The novel concept of 'logical transmogrification' plays a central role in this paper, but only on page 8 is it actually discussed or defined. This left me lost for the first half of the paper. The concept should be clearly described in the introduction. Also, Section 3 defines the proposed method, but provides no examples nor intuition to aid readability. Some examples would greatly improve this section. ...” | 
|	“The paper is uninteresting”
<br><br>
(No justification or details provided.) | 
	“The paper proposes a method to generate pseudorandom numbers from RDF triples, but it is unclear to me what such a method is useful for. It would be helpful if the authors could highlight concrete use-cases for such a method in the introduction, along with a motivating example.” |
|	“The contributions are not clear”
<br><br>
(No justification or details provided.) |
	“The title and introduction of the paper focus on data quality, but the techniques described and evaluated in the rest of the paper seem to apply standard OWL reasoners over the data for motivations that appear to me largely unrelated to data quality. The authors should clarify their contribution in the introduction and ensure that it reflects the content of the paper.”|
                
### Be civil and polite  {#BeCivilAndPolite}
                                                
Please keep a civil tone. Though (almost) nobody sets out to be uncivil, it can be challenging to avoid indeliberately coming across as being “harsh” in anonymous reviews. Keep in mind that you may be reviewing the papers of students who are new to research and the community, or more generally, the papers of authors who have invested a lot of time and effort into their work. Your review should be constructive. Your review should include discussions of both positive and negative aspects rather than focusing only on negatives. Your review should not be disparaging or dismissive, and should avoid unnecessarily negative language. Until proven otherwise, you should assume good faith on the part of the authors. Avoid calling into question the ethics or honesty of the authors, but rather keep your review factual. If you have an ethical concern regarding a paper, please discuss it with other PCs or the FroCoS chairs.                         
                                        
Examples to avoid
	Better examples
	“The writing is terrible”


(Unnecessarily disparaging and dismissive. Not constructive.)
	“The writing contains frequent spelling mistakes and grammatical errors, making it hard to follow and review. Below I will provide some samples of these errors to illustrate the types of mistakes I hope the authors can fix for a future version.”
	“The authors clearly have little understanding of the area.”


(Unnecessarily disparaging and dismissive. Not constructive. Not justified. Speculative.)
	“The paper makes claims that contradict the literature, for example, that Horn Description Logics do not support range restrictions. The related works section misses some key references [A,B,C] for EL. The authors should consider [C] as a survey of the relevant literature, if they have not seen it.”
	“The experiments were selected to make the authors' approach look good.”


(Assumes deliberate dishonesty when other possibilities have not been ruled out.)
	“The paper does not justify why the authors create a benchmark of their own formulae (with shallow nesting), nor why they did not use an existing benchmark such as proposed by Roe et al. [A]. The latter benchmark has been used in many works and includes formulae with a varying nesting depth, for which I suspect the authors' approach will not work as well relative to the baselines. Including an external benchmark would help to examine these cases and solidify the papers' claims.”
	

### Adequately justify your recommendation   {#AdequatelyJYRecomm}
                                
Please clearly relate your review comments to your recommendation. The authors do not necessarily need to agree with your recommendation, but they should at least be able to understand your rationale, and how you think they could improve their work.
Each paper should satisfy the relevance criteria of the call, advance the area by providing significant novel insights/claims (which may include negative results), be technically correct in terms of its key contributions, be understandable and (when applicable) reproducible by someone knowledgeable and patient, and provide enough evidence to justify its key claims and conclusions. Failing (in part or whole) with respect to one of the criteria in the call for papers is potentially a valid reason to reject. Keep in mind that papers can achieve these goals without being highly technical and while leaving open questions or tasks for future work.
In case you recommend a reject, ensure that you clearly justify the rejection. Avoid rejecting a paper solely 
* For infrequent minor issues that do not affect the key content of the paper, but can instead be addressed by the authors (in an obvious way) for a camera-ready version.
   * Rather make your recommendation assuming that infrequent minor issues are corrected. Make concrete suggestions on how to address these issues for a future (possibly camera-ready) version of the paper.
* Because you think you know a better way to address the problem.
   * Rather base your recommendation on the proposed approach, and suggest exploring the idea for future work (if you are happy to share it).
* Because there is something it does not achieve.
   * Rather base your recommendation on what the paper does achieve, and whether or not that is correct, sufficient, etc. Do, however, expect key limitations and scope to be adequately clarified.
* Because there exists a benchmark or baseline not used in the experiments.
   * Rather base your recommendation on whether or not the experiments and/or proofs are sufficient to justify the key claims or conclusions of the paper, and whether or not those claims/conclusions are of importance.
* Because the results are negative.
   * Rather base your recommendation on whether or not it advances the state-of-the-art, or offers negative results that provide novel insights on how the state-of-the-art can be advanced in future.
* Because it is not clear how its results could be immediately put into practice.
   * Rather base your recommendation on what the community stands to learn from the paper.
* Because it does not appear highly technical, or because the method (in hindsight) appears “obvious” or “trivial”.
   * Rather base your recommendation on whether or not the paper provides novel ideas or insights that advance the field.
* For not meeting unrealistic, arbitrary or open-ended goals.
   * Rather base your recommendation on realistic and/or concrete criteria that are justified in the context of the goals of the work and the literature.
We also ask reviewers to refrain from later changing (only) their recommendation to “follow the crowd” or to “seek consensus”, particularly when the new recommendation is no longer justified by the review text. However, if during the discussion phase with other reviewers and chairs you see something in a new light, or agree with another reviewer regarding a certain positive or negative aspect, you may of course change your recommendation, and modify your review text accordingly. We aim for real consensus on papers where the reviewers stand by their recommendations. Failing that, we prefer no consensus to an artificial consensus where recommendations are changed just for the sake of aligning them.
                                                
                                
                                
                                
                                        
Examples to avoid
	Examples to follow
	“This paper must be rejected due to having multiple typos, missing references to similar works in related areas, and bugs in Equation 1.”


(All such issues have clear resolutions that could be easily addressed for the camera-ready version. Few specific details are provided to justify the recommendation or improve the work.)
	“For a future version of this paper (potentially the camera-ready version, if accepted), the authors should be sure to address the following minor comments:


Please spell-check, e.g., 'qeury', 'frgment', etc.The authors should acknowledge similar works in relational databases, e.g., by pointing to the survey of Roe et al. [A]. In Equation 1, max should be replaced by arg max.”

OR


“The paper has many grammatical errors and notational bugs that made it difficult for me to follow and review. I fear that other readers, even experts in the area, would likewise have difficulty understanding the work. For this reason I recommend a reject. Below I will provide some illustrative examples of these issues, which should be addressed for a future version”
	“I am rejecting this paper because one could obviously achieve better performance in Algorithm 1 by parallelising the branches.”


(This is speculative. It is best offered as a suggestion for future work, rather than a reason to reject. The suggestion might only be obvious after reading the paper.)
	“As part of future work, I think it would be interesting to explore the idea of parallelising the branches in Algorithm 1, which may lead to further performance improvements.”
	“One argument for rejecting the paper is that the current approach does not support updates, which are crucial in practice.”


(Even though updates are important and not considered, the approach could be extended in future. The justification for rejection should consider what is presented, not what is not presented.)
	“The work achieves impressive results for the read-only case. Though a complete solution would require support for updates, the authors discuss how such features could be combined with the proposed approach in future.”


OR


“One reason for rejecting the paper is that the current approach does not support updates, and there is no clear way in which the method could be extended to support updates due to the nature of the data structure proposed. The paper does not discuss this issue. While a highly-optimised read-only index might still be a useful contribution, the approach proves to be only marginally faster than baselines that do support updates.”
	“The paper does not deal with the case of cyclic graphs, and hence I recommend rejection.”


(Even without considering the cyclic case, the results for acyclic cases might be an important contribution. The justification for rejection should consider what is presented, not what is not presented.)
	“The paper proves a novel tractability result for the case of acyclic graphs using new techniques. This begs the question of what happens in the cyclic case, which seems an interesting direction for future research based on these results.”


OR


“While the paper proves a novel tractability result for the case of directed acyclic graphs, it is a minor extension of a similar result by Boe et al. [A] for trees, and uses the same techniques.”
	“I recommend rejecting the paper as the benchmark from Doe et al. [A] is not used and the authors include only two baselines.”


(It is not clear what the additional benchmark would add to the discussion. The baselines the reviewer wishes to see are not specified, nor why these particular baselines are specified. It is not made clear why extra baselines are needed or what they would add to the discussion. It is not clear that it would be feasible to run them. It is not clear what claims are not properly validated, but would be validated with these additional experiments.)
	“The paper's selection of baselines and experiments, though incomplete, provides strong evidence for the claims of improved performance for path queries.”


OR


“I recommend a reject because the paper claims to provide superior performance versus the state of the art for regular query answering, with a main contribution being the optimisation of path queries. However, the benchmarks tested include very few path queries. To validate these claims, it would be necessary to include a benchmark with more (diverse) path queries, such as proposed by Poe et al. [A], in order to better understand the performance of such queries. Also, the baselines included run on disk while the proposed approach runs in memory. A fairer and stronger baseline would be to compare with the in-memory database proposed by Joe et al. [B], which is optimised for path queries, and has a code repository linked from the paper.”
	“The paper reports a precision measure of 46%, which is far too low for the approach to be applicable in practice.”


(While this may be true, the paper may still improve upon the state of the art for a challenging and important problem. It may lead to further developments that, in turn, lead to approaches applicable in practice. Alternatively, the paper may be reporting an interesting negative result that refutes a commonly held belief/misconception within the community.)
	“The paper reports a precision measure of 46%, which though still too low for most practical applications, is a significant improvement with respect to the state of the art on this challenging and important problem. I think that further improvements can follow from this work, and can eventually yield more precise techniques that are applicable in practice.”


OR


“The paper reports a precision measure of 46%, indicating that Deep Learning methods are outperformed by much simpler classifiers for this task. This is quite a surprising negative result! The ablation study provides very useful insights into why this is the case.”


OR


“The paper reports a precision measure of 46%, which is too imprecise to be useful in practice, and offers only a single percentage point improvement over the baselines tested. On the other hand, recall drops by several percentage points compared to these baselines. Given the somewhat incremental nature of the proposal, and the arguable performance improvement over the baseline method, I lean towards rejecting this paper.”
	“I recommend rejecting the paper. Though the approach is new and proves effective, it is also trivial and fairly obvious. It was not difficult to come up with this approach.”


(Exploring and reporting on “obvious” lines of research is important to advance the community, and often an approach that appears “obvious” is only so in retrospect. Such ideas that provide new insights through simplification are often crucial ideas for advancement. How easy or difficult it was to come up with the approach is subjective and speculative.)
	“The approach is not only effective, but it is also quite natural and elegant. It is surprising that nobody has thought of this approach before, and I commend the authors for not only coming up with this idea, but evaluating and publishing it.”
	“I think the paper should be rejected as discussion on related works is selective and brief. I can name around 30 to 40 references that were not discussed. Also the new benchmark that the authors created by hand only contains 10,000 examples, which is insufficient for training deep neural networks.”


(Goals appear unrealistic. Due to space reasons, conference papers cannot reference and discuss every potentially related work. Even dedicated surveys will sometimes miss references. No specific missing references are mentioned. Creating an even larger benchmark by hand appears to demand too much of the authors. Having more than 10,000 examples is an arbitrary goal: if the authors had 20,000, would this be enough, or would the review still ask for more? What would be enough, and why?)
	“The paper does not discuss all of the papers in the area, but rather focuses on more recent approaches to the problem using similar machine learning methods. This is understandable for space reasons, but I would recommend at least including the seminal works by Boe et al [A] and Foe et al. [B], and if space permits, works by Koe et al. [C,D] as well.


It is commendable that the authors create a new benchmark of 10,000 examples for this problem, which is a useful contribution to the community! However, the dataset by Toe et al. [A] contains 50,000 examples, and is commonly used for training deep neural networks. If the authors' dataset could somehow be extended in future to a similar size, perhaps using a similar methodology on a crowdsourcing platform, it could replace that dataset with much higher-quality examples.
	

### Be honest about your understanding of the paper   {#BeHonestAYUnderstandingOfThePaper}

Of all the guidelines, this can be the hardest to follow. As much as we can try to avoid this situation, it can happen that you are assigned a paper that is a bit outside your comfort zone or area of expertise. Or you may be assigned a paper in your area that contains a large amount of technical detail you cannot verify in the time given. Please do not give up right away. Try your best to understand as much as you can of the paper, and to provide a recommendation based on what you understood. Be honest in the review text about what you understood, and what you didn’t understand. It is possible that someone more expert in the area might find the paper really interesting and worthwhile. Conversely, and perhaps even more commonly, your lack of understanding might well be the paper’s fault: it might be the case that the paper uses unhelpful notation, over-complicates technical detail, is poorly written, etc.
Even if you do not have much experience in the particular sub-area, be wary of papers where you struggled to follow the motivation, overall technical ideas, and main results. These should be expressed in a manner that the broader FroCoS audience can understand. Be particularly wary of papers for which other reviewers also expressed major difficulties understanding (something that can only be detected if reviewers are honest about their understanding of the paper). If the chairs feel that a more expert review is necessary, they will solicit it (something that again depends on reviewers being honest about how much you understood).

If you did not fully understand a paper, please consider lowering your confidence score. When assigning the score, please take into account the following aspects:
- Your depth of understanding of the paper.
- How well you know the literature in the area.
- How certain you are about your recommendation.

Please try to be honest and fair when selecting your confidence, which is intended to be a measure of the previous three points only (and not your repute as a researcher). The scores can be interpreted as follows (based on guidelines for ACL 2014).
- 5: (expert) Positive that my evaluation is correct. I read the paper very carefully and am familiar with related work and have published on this topic.
- 4: (high) Quite sure. I tried to check the important points carefully and am familiar with related work. It’s unlikely, though conceivable, that I missed something that should affect my ratings.
- 3: (medium) Pretty sure and willing to defend my evaluation, but there’s a chance I missed something. Although I have a good feel for this area in general, I did not carefully check all the paper’s details, e.g., the proofs, experimental design, or novelty.
- 2: (low) It is quite probable that I missed some details, didn’t understand some central points, or can’t be sure about the novelty of the work, since the topic is peripheral to my own interests.
- 1: (none) Not my area, or the paper is very hard to understand. My evaluation is an educated guess based on general understanding of science and scientific writing.

While in an ideal world all reviews on a paper would provide genuinely expert comments and recommendations, in practice, this is quite a rare situation, even for experienced reviewers/researchers. In case of lower confidence, we encourage you to indicate in the review (or the internal comments to PC/chairs) issues relating to your understanding of the paper, your knowledge of the area, or doubts you may have about the recommendation. Such comments may be crucial for making fair decisions on which papers to accept, and which to reject.                                        


## Suggested review structure   {#SuggestedRevStructure}

Most reviewers have developed their own style of review over time, and no individual style is “best”. But if you are a relative newcomer to reviewing, and are looking for guidance on how to structure your review, consider adopting the following structure:
* Overview: Summarise the paper in your own words in a short, concise paragraph. While the authors (presumably) already know what their paper is about, this demonstrates to the authors, other reviewers, and chairs the extent to which you understood the paper, and what your personal perspective of the paper is. If you can provide a good overview, the authors will tend to value your opinion more. It is also a good exercise to ensure that you understand the paper. (In case there are parts of the paper you did not understand, clarify them here.)

- Strengths: Summarise around three main strengths of the paper as concise bullet points. Being able to expand on the positive aspects of the paper can be encouraging to authors, and can also help them to improve their work by building upon those strengths.

- Weaknesses: Summarise around three main weaknesses of the paper as concise bullet points. You do not need to go into too much detail yet. Do not include minor issues here. Consider criteria as listed in the call and in the questions of the review form (e.g., relevance, impact, clarity, reproducibility) when preparing the list of weaknesses.

- Detailed comments: Discuss in more detail each of the weaknesses. As a guide, you could aim for a paragraph on each weakness. Relate each weakness to specific aspects in the paper. Relate them to the criteria in the call for papers, if necessary. Be constructive, polite and factual. Always try to clarify how the authors could realistically address these weaknesses, providing details. If you cannot clearly justify your reason for listing a weakness here, remove it.

- Recommendation: Explicitly state your recommendation (reject, borderline, accept, etc.). Relate your recommendation to the aforementioned strengths and weaknesses. Almost every paper, even strong ones, have weaknesses. Not all weaknesses are grounds for rejection. Some might refer to limitations that could be addressed for future work. Other weaknesses might be adequately addressed as part of the camera-ready version (e.g., being more upfront about certain limitations). In case you accept, make clear what improvements (if any) you expect for a camera ready version. In case you recommend a rejection, provide a summary of directions in which the authors could improve their work.

- Minor comments: Provide here minor comments that seem to have an easy and uncontroversial fix, such as spelling mistakes, grammatical mistakes, bugs in notation. In case such errors are frequent, you can opt to provide 3-4 illustrative examples, and also list the general issue as a weakness above (e.g., if frequently poor grammar makes the paper very difficult to understand, make that a key weakness).
