# Technical Writing

The below is a rather loose list of thoughts stemming from my own experience as technical writer, reviewing tons of academic papers, and student dissertations.


## General Guidelines

* **G1—Start early.** Writing is closely linked to thinking and if you cannot write about something, you haven’t understood it. Hence, starting early (e.g. * with an introduction) helps you clarifying many things.
* **G2—Space = time = importance**. Reading text takes time. The more space a text takes, the longer it is, and the longer it takes to read. When writing parts of your paper, think of the space you attribute to a text as proportional to its importance as it defines how long a reader will deal with this part. The most important implication of this is that you should detail the parts that talk about your work, while shrinking the parts that do not talk about your work. An exception is abstract and introduction. They are very important, but therefor they stand in the beginning. Still, keep them short and to the point as they are not contributing anything.
* **G3—Iterate**. Iteration will reflect the pace of the evolution of your thoughts and help evolving them in return. You will automatically improve with each step. And in case you are not improving, then you have a strong case that the previous version was perhaps better. You can reset or retry. Both will help you improving. Iteration is in particular important for the introduction. Even the very successful writers and researchers write several introductions. It’s perhaps the hardest part of each paper.
* **G4—Reference Figures**. Though everyone likes figures and more so ‘browsing just the figures’, figures are not part of the text. They are figures while the text is a linear and logical unit. If you are including a figure, reference it and explain it. A figure is not there for illustration but to help you making the point for the reader; to help him understanding. Think of the moment in a presentation when you show a specific figure. Without referencing the figure, the reader will most likely not look at it and hence lose the message. More important, the text should be understandable almost without the figures.
* **G5—Do not make the reader think.** Be explit. If you have to think a lot when reading someone’s text, how likely are you to continue reading? Exactly. Thus, don’t make your readers think. Be explicit, even if it takes space and better add one or two additional explanations or examples that help following your point. You can ask a colleague later if it’s too lengthy and if you should remove parts. Removing is always easy and you will get a good feeling over time.
* **G5—Inform**. The objective of technical writing is not to entertain the reader, but to inform. Readers are not reading your work to bridge their time, but invest their time to read your work. Hence, be to the point and help them saving time. The less it takes them to understand your work, the longer their will read it (and cite!).
* **G7—Detail your methodology**. Your methodology is everything the reader has to assess your credibility. Without methodology, you might as well have made up all the results and created the pictures in photoshop. Where are your results and conclusions coming from? A strong methodology adds credibility to your results. Having asked 1,000,000 people about whom they will vote for gives a much stronger result than having asked 10; having asked people in different parts of the country will be stronger than having asked your best friendsl; having designed 5 prototypes implies you have learned more than having designed 1, etc. Thus, a good methodology explains the details (details are important and show that you have really done it and thought it through), highlights the strong points (how many participants, what background, etc..), and explains why each step was necessary (and not another one).

## Random Things

The below advice is collected from many recurring errors in students' writings.

* Try to avoid implicit references such as 'this'  or 'as discussed above' or alike. Use explicit references by repeating the term you're referencing.
* Label your figures and include meaningful captions that explain the figure in sufficient detail.
* In English, there is a blank ' ' before any opening bracket; there is no blank ' ' before : (as it is in French)
* By early August you should spend more time writing than implementing. - Keep some of the polishing bits to the end when you're done writing. 
* Keep in mind to demonstrate your solution: this includes figures and can be videos, too. 
* the report is what the reviewer will see. They will not know about our discussions nor anything else. Anything you do not mention 'did not happen'
* at the same time, do not bore with details. Do not explain any little change during your iterations. Only add the information relevant to understand and assess your contribution / solution / research question. I will not be able to tell you what that is. You will have to decide that. 

## Possible Outline and Section Content

The below structure follows the standard in technical writing. You can use it as a check list when preparing your submission. However, there are many cases you may want to adapt the structure. If you are in doubt, the best is to stick to this structure. It mostly works. (Duplications in the below list are on purpose -> space=time=importance).

### Abstract
The abstract should reflect the following structure:
* WHAT -> What is the paper contributing?
* WHY -> Why is this important?
* HOW -> How did you do it?
Results -> mention the 1-2 most important findings of your research.

Example:

_We report on a controlled user study comparing three visualization environments for common 3D exploration. Our environments differ in how they exploit natural human perception and interaction capabilities. We compare an augmented-reality head-mounted display (Microsoft HoloLens), a handheld tablet, and a desktop setup. The novel head-mounted HoloLens display projects stereoscopic images of virtual content into a user’s real world and allows for interaction in-situ at the spatial position of the 3D hologram. The tablet is able to interact with 3D content through touch, spatial positioning, and tangible markers, however, 3D content is still presented on a 2D surface. Our hypothesis is that visualization environments that match human perceptual and interaction capabilities better to the task at hand improve understanding of 3D visualizations. To better understand the space of display and interaction modalities in visualization environments, we first propose a classification based on three dimensions: perception, interaction, and the spatial and cognitive proximity of the two. Each technique in our study is located at a different position along these three dimensions. We asked 15 participants to perform four tasks, each task having different levels of difficulty for both spatial perception and degrees of freedom for interaction. Our results show that each of the tested environments is more effective for certain tasks, but that generally the desktop environment is still fastest and most precise in almost all cases._

### Introduction
The introduction is perhaps the most important part of your paper. Take specific care of it. Most people won’t necessary read beyond the introduction and based on abstract and/or intro will judge whether to cite or in the worse case reject your paper. The introduction sets the tone. If you do a good job in detailing your motivation, method, and contribution, your work gains credibility.
Different from the abstract, the introduction usually follows the slightly adapted structure:
* WHY
* WHAT
* HOW

Within this structure, cover the following:

* **Contribution:** What is novel and why would people cite your paper. The best is to dedicate a paragraph to the contribution. You may want to iterate and refine as you go. This is usually a paragraph that starts with 'In this paper .. '.
Type of contribution: are you presenting a survey, a controlled study, a system, a case study, etc..
* **Methodology:** how did you structure your work, what high-level steps did you undertake that helped you coming to your conclusion/result.
* **State outcome and impact:** what did you eventually find and who benefit from it. This can be a single brief sentence.
Mention URL to additional material, if available. Readers who don’t read your entire paper will still find the ‘fun’ bits. It’s generally a good idea to provide a website or simple blog (e.g. WordPress) alongside with your work. This helps the lay-reader to better understand what you have done. Add pictures, working code, etc.
* **Mention external collaborators if present**. This strengthens your method and credibility from the beginning on.
* A **research question** can help the reader understanding your goal and methodology. A research question is a question that you can answer with your methodology.  You can state the question explicitly: ‘We are interested in how people use pen and paper to annotate visualizations.”


### Background / Related Work

This section, usually following the introduction provides the knowledge the reader needs to know to understand your contribution. A good background section can support your motivation of why this research is necessary as well as support your contribution to the state-of-the-art. Write the related work with these objectives in mind.

Calling this section ‘Background’ or ‘Related Work’ depends a little. There are no real rules when to use which term. I would use background if I have to talk about general knowledge such as the description of a domain my work is situated in (e.g. protein interaction, peace agreements, Islamic History, etc..). Here you want to talk about specific terminology, previous work, and current challenges. In a related work section, your focus is on related research addresses a similar goal or question than you. 

If it is not clear from your intro which areas you are covering in your thesis, start your related work with a brief overview which areas you are talking about and why.

Your related work should tell a story. Don’t start with the references and write a ‘laundary-list’ of the form ‘X did blah‘. This is of very limited information. It means you have read all of them (never cite without reading the paper), but you have not understood the larger picture. Start from the larger picture and tell us what are the main trends/technologies/concepts are related to your work. Then, insert the references were you need them. If a reference doesn’t fit, it probably isn’t important. Or, you’re missing a part of the story.

Also, balance detail and brevity. Some references are more important than others. Talk about the more important in more detail, while keep the less important to the minimum. It’s ok to reference 2 or even 3 sources in one sentence, e.g., “other approaches had yielded similar results [1,2,3]”. 

Relate your work on the related work (hence the name). Make this relation explicit and don’t let the reader think (G5). If you can’t tell what’s the difference, search for arguments and make it clear. It shows how your work advanced and complements existing work. It also shows that you know why you are doing something specific and that have the knowledge of the literature to judge your contribution.

### Discussion Section ('Discussion')

Discussions have two purposes: reflection and outlook. Reflections critically discuss your own work, its achievement, and limitations. Research is flux and each work (should) bring some certainty and some more knowledge about the uncertainty we’re facing with this certainty. What did you we (you) learn? What are the unsolved problems (technical, conceptual, global) and what are the things you can talk about with some more certainty. During writing, it helps listing candidates for a discussion. When you finally write that section, you will know better what you can keep and what to drop. You do not have to discuss everything.


### Conclusion/Summary
This can be short, summarizing your achievement and tell what others can do with your great work.


## Literature Search
Reading papers and keeping track of it can be overwhelming as there are so many papers out there the internet will give you access to tons of results and even more links to related ones, and most papers sound relevant in the first place. Below are my personal notes and strategies to cope with the flood of potential literature. Try to read as much as you can but do not be afraid if you have not read everything. You need a good feeling for what is relevant and what is not. Not everything you read will be relevant for inclusion into your paper/thesis.

### Where to Find Papers?
* Use key terms in [Google Scholar](https://scholar.google.com)
* Look at forward citations, i.e. papers that cite a relevant paper
* Look at backward citations, i.e. papers referenced in a relevant paper
* Look at recent conference proceedings (for us that’s mostly likely IEEE VIS, EuroVis, PacificVis, ACM CHI).

### How to keep track of papers:
* keep one google document
* list all the papers you find interesting to potentially read, ordered by some means (e.g. years, first author last name, title etc.)
start reading the most relevant. You don’t need to read the entire paper. Start with the abstract, then intro and go as far as you like. Take notes for each paper you read in the gdoc under the respective title.
* Include the URL for the paper in the gdoc.
* if you come across interesting papers referenced in the paper you read, add their title into the gdoc.
* once finished reading a paper, pick a new one and so on.
* To me, this provides a good overview of the papers I have already read, and the ones I potentially want to read. Looking at the listed titles, I can decide which ones are the most important to read next. Also when I add a new title to the collection, I sometimes add two types of brief comments
* how relevant I think the paper is, at the moment where I find it, and
* if I find a paper references in another paper, I usually add a comment what that paper said about the referenced paper (e.g. a study showing X). That, too, helps deciding later how relevant that paper is to be read.
* You can use citation management systems such as [Zotero](https://www.zotero.org/).

# Evaluation
* high-level question
* hypotheses and questions (H1, H2, H3, ...)
* conditions and techniques being tested
* Tasks for participants to do
* study design: what is your study protocol: first, we did X, then we did Y, for X minutes, ... 
* participants and demographics whatever is helpful for your resarch
* Results. This is very objective analytics. Don't inculude interpretations or discussions
* Discussion



 



