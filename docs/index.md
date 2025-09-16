# Nmbrs Partner Portal 

This documentation site is a Proof of Concept of how Nmbrs could provide a dedicated user experience for partner developers that work on HRIS integrations and make the API handling easier through guides, use cases and best practices. 

To do this, I built an MkDocs-based portal with the help of ChatGPT, to illustrate how documentation could evolve into a real **Partner Portal**.

---

## Step 0 — Documenting my thought process

### Why I chose this solution
I wanted the partner developers to feel accompanied through every step of their integration journey. 

A portal that consolidates partner content in one location that is (ideally) designed with an approachable look and feel can:
  - Make the user feel like they know where they're going and not wasting time looking for information in different portals and sources
  - Enable partners to easily browse guides by use case
  - Fill information gaps by providing additional tips and best practices
  - Go beyond endpoint reference by including real-life applications

I used MkDocs (Material) because I am familiar with the tool to prototype quickly and use components such as: tabs, admonitions, search, dark mode, code blocks, buttons.

### Challenges faced
- Understanding the product, user, end user and the integration workflow. I had to learn the basics of a new system in a short amount of time. But this is a part of the job.
- I spent a good amount of time trying to access the API Mock Server so I could test the APIs. I believe their solution is no longer maintained, because the environment that I was meant to see in Postman no longer seemed to exist. To save time I opted for using the default payloads and responses documented in the API reference. 
- Documentation was spread out across different sources. It was hard to follow a coherent path, I had to look for information on several websites and pages. 

#### What I’d do differently 
- I would've brainstormed with my (in this case, imaginary) team to help me decide on priorities. I had several ideas and at times got carried away. Having people to bounce ideas off of helps me make decisions faster.  

### How I behave in real projects
- First I sync with a Product Owner to ensure I have:
    - Test access to the feature
    - A list of limitations, if any
    - An overview of a practical use case for the feature
- Define if all supporting content already exists, and if it doesn't, create it
- I test the feature and document as I go
- Give feedback on potential bugs
- Identify potential sources of difficulty or errors that the user might face and prepare for that - include warnings and tips in the documentation
- Keep in constant contact with stakeholders in case I have any questions
- Personally review the finished documentation and submit it for peer review

#### Questions I would ask the Product Owner or a developer
I had a couple questions specific to the API while documenting, I decided to share them to give you an idea of what questions I'm likely to ask a Product Owner. 

- Is it possible to create users in bulk via the API? I imagine that for a data sync use case, it would be useful if the partner developer could add many users at the same time. 
- Are there permission requirements for API access and integrations? I could not find this information.

---

## Step 3 — Roadmap to reduce “getting started” support load

**Goal:** Enable partners to self-serve by turning isolated endpoints into **scenario-driven guides** (with runnable examples, a new content structure and troubleshooting).

1. **Capitalize on existing content (Week 1)** - Create guides that group all content distributed across different sources in one place. This is existing content that can be adapted and pages that will include explanations of global API concepts. The specifications for the last can easily be found in different online sources. 
    
    **Impact:** Centralizing guides that are a requirement to use the API creates a single source of truth and reduces time - Technical Writers can link to these guides in the requirements and only have to update the source. 

2. **Create an interactive prototype (Week 1)** - Create a temporary repository and website (with open source tools like Mkdocs) to illustrate the idea and have a space partners can test the content (refer to step 4). 
    
    **Impact:** allows users to imagine a different content structure, tone and a different way of interacting with APIs, separate from the existing documentation to avoid biases. 

3. **Contact Support (Week 1)** - Concurrently gather data from support team to define a list of the 5-10 most asked questions and issues encountered when integrating.
    
    **Impact:** start gathering real user data as soon as possible so we have enough to animate the iteration phase (step 5 of the roadmap)

4. **User Tests (Week 2)** - Find one or more partners to test the prototype docs end-to-end and carry out a user test to collect feedback. Have different stakeholders test the prototype and give feedback as well.
    
    **Impact:** seeing how the user interacts with the content in real-time and getting fresh, honest feedback.

5. **Current state assessment (Week 3)** - List all features approved and suggested by users and cross-reference with the list of features and components of the content platform currently used. If too many differences are identified, set up a meeting with front team (see the last step).
    
    **Impact:** understand the limitations and/or advantages of current content platform and assess how long it would take to implement new content structure. 

6. **Apply and Integrate (Weeks 4-5)** - Transform the data collected during steps 3, 4 and 5 into action items for content iteration, improvement and expanding the content to document new use-cases. Ideally we integrate the content created for the prototype and any new content into the existing documentation - adapting what can be adapted and getting creative when it is not possible.
    
    **Impact:** An amalgamation of all impacts up to now. 

7. **Frontend Team Collaboration** - Contact the Frontend team about the possibility of creating a dedicated partner portal website. Show them the prototype and assess if a similar, but more secure and scalable solution is possible and when. Create a new roadmap if the answer is yes. If it is no, put the project aside until next opportunity and continue brainstorming on how to creatively integrate user feedback into existing content platform. 

8. **Continuous iterations** - Repeat steps 3, 4 and 6 *ad infinitum*.
