Natura DevOps - Challenge
==========================

Hello and thanks for taking the time to try this out.

The goal of this test is to assert (to some degree) your coding and architectural skills. 
You're given a simple problem so you can focus on showcasing **dev** and **ops** techniques.

As this is a review process, please avoid adding generated code and manifests to the project. 
This makes our jobs as reviewers more difficult, as we can't review files that you didn't write it. 
This means avoiding committing vendor folders or similar, which generates thousands of lines of code in stub files.

_Note: While we love open source here at Natura &Co, please do not create a public repo with your test in! 
This challenge is only shared with people interviewing, and for obvious reasons, we'd like it to remain this way._

Instructions
-----

1. Fork this repository.
2. Create a pull request from your branch to the master branch. This PR should contain setup instructions for your application and a breakdown of the technologies & packages you chose to use, why you chose to use them, and the design decisions you made.
3. Reply to the thread you're having with our HR department telling them we can start reviewing your material (please include PR number).


Task
----

- Assume you are running on your favorite cloud (Azure, AWS, GCP)

- Create a README.md that outlines your line of thinking for the solution
- Create terraform, docker and kubernetes resources
- Suppose these apps will run on blackfriday week, assume daily bell-curve scalling.
- We want to deploy two containers that scale independently from each other
    - `Container 1:` This container runs a small API that returns data from S3
    - `Container 2:` This container runs a small API that returns consultant information from a database
- Please be aware that you can use any docker image you'd like for your containers. It's just an example. What we're truly seeking here is how you will consider in all of those manifests asked above.
- For the best user experience auto scale the `Container 1` when CPU average reaches 70%
- For the best user experience auto scale the `Container 2` when Memory average reaches 70%
- Ensure the deployment can handle deploys and rollbacks
- How would you apply the configs to multiple environments (e.g. staging x production) ?

####  

Evaluation Criteria
--------------

1. The problems are solved efficiently and effectively, the application works as expected.
2. The application is supplied with the setup scripts.
3. The application is well and logically organised.
4. The submission is accompanied by documentation with the reasoning on the decisions taken.
5. The code is documented and is easy to follow.
6. The answers you provide during code review.
7. An informative, detailed description in the PR.
8. Following the industry standard style guide.
9. A git history (even if brief) with clear, concise commit messages.
10. Architecture Drawing
11. We will evaluate what you commit in this repo. You do not need to keep anything up in your personal Cloud Account.

---

Good luck!
