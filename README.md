# USWDS proposals

> **Note**
> At this time, we are accepting proposals only for new components. 
>
> You can [submit requests for new features or enhancements](https://github.com/uswds/uswds/issues/new/choose) by creating an issue in the uswds repo.

This repo acts as a public hub to submit and discuss proposals for new U.S. Web Design System (USWDS) components.

## Overview of the proposal process

All requests for new USWDS components must be submitted as a proposal. Proposals are detailed documents that should make a compelling case for adding a new component to the Design System.

Anyone can submit or contribute to a proposal. Community contribution is at the heart of this process and we encourage you to share your ideas, opinions, and votes.

### Ways to contribute

The proposal process exists to help the USWDS team better understand community interest in new component ideas. Your opinions matter, and we want to make it easy for you to contribute.

To help guide you through the process, we provide the following resources:

- [Instructions for submitting a new proposal](#submitting-a-new-proposal)
- [Instructions for contributing to an existing proposal](#contributing-to-an-existing-proposal)
- [A proposal template](https://github.com/amyleadem/uswds-proposals/blob/main/proposals/_proposal-template.md)
- [Information about our evaluation process](#proposal-evaluation)
- [Roles and responsibilities](#roles-and-responsibilities)

#### Help with GitHub

This process requires a knowledge of GitHub [branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches) and [pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests). If you need help submitting or contributing to a proposal, please reach out via [TK].

## Submitting a new proposal

When you are ready to propose a new component for the Design System, you'll need to submit that idea in the form of a proposal. We provide a [proposal template](https://github.com/amyleadem/uswds-proposals/blob/main/proposals/_proposal-template.md) to help guide you through the process. When filling out the proposal template, there are a few things you should know:

**It’s okay to start with the basics.** We understand that you’re busy and might not have the specialized resources to thoroughly fill out every section of the proposal template. If right now you can only summarize your idea and provide a simple explanation for why it is a good addition, that’s great! Submitting an incomplete proposal gets the conversation started and creates a central location to gather thoughts and information from the community.

**A proposal must be fully filled out before it can be considered for inclusion in the Design System.** Completed proposals are thorough documents. A complete proposal should make a detailed, compelling case for the new component. Every section should be filled out. If a proposal is lacking critical information, it will be sent back for revision. 

### How to create and submit a new proposal

1. **First, check if a proposal for your idea already exists.** You can do this by looking at the [pull requests in this repo](https://github.com/amyleadem/uswds-proposals/pulls). If a proposal for your idea already exists, that’s great! You can contribute to the conversation by adding comments, information, and voting. You can learn more about [how to contribute to an existing proposal](#contributing-to-an-existing-proposal) in the next section.

1. **If a proposal doesn't exist, it's time to create one.** Here are the steps to do that:
    1. **Create a new branch.** [Create a new branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) for your proposal named: `[proposed component name]-component`. For example, if you wanted to propose adding a loader component, you would name the branch `loader-component`.
    1. **Copy the proposal template.** In your new branch, create a file in the `proposals` directory called `[component name]-component.md`. For example, `loader-component.md`. Copy the contents of [proposal-template.md](https://github.com/amyleadem/uswds-proposals/blob/add-readme-and-template/proposals/proposal-template.md) into this file.
    1. **Fill out the template to the best of your ability.**  An asterisk (*) in the template indicates a required field. All required fields must be complete before your proposal can be considered for the Design System. However, to initially submit a proposal you must only complete the “Summary” and “Motivation” sections. You or someone else can finish the rest later.
    1. **Open a pull request.** [Open a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (PR) with the title: `Proposal: [Component name]`. For example, `Proposal: Loader component`. Once your PR is open, it will receive a "Status: Submitted" label and will be available for voting, comments, and additions.

1. **Get the conversation started.** Once your PR has been opened, invite others to participate in the discussion and add information. Use the [uswds-public Slack channel](https://gsa-tts.slack.com/archives/C3F14AHSQ) or reach out to peers to solicit feedback and support.

## Contributing to an existing proposal

Every proposal can benefit from community input. If you would like to help with existing proposals, we encourage you to contribute by:

- [Voting for proposals](#voting-for-a-proposal)
- [Adding information, research, and solutions](#adding-information-to-an-existing-proposal)
- [Sharing ideas and asking questions](#sharing-opinions-and-asking-questions)

### Voting for a proposal

One of the easiest and most effective ways to express your opinion about an idea is to vote. The votes a proposal receives can quickly communicate the community's general level of interest in an idea. This can help inform which items the USWDS core team will look into first.

To vote for a proposal, you simply need to add an emoji to the proposal's PR description by clicking on the smiley face in the bottom left corner of the description box. Here’s what each emoji communicates:

| Emoji            | Action | Description |
| :----------------------------: | :-------------- | :--------- |
| 👍 | Up-vote |   A thumbs-up emoji means that you support including the component in the Design System.    |
| 👎 | Down-vote | A thumbs-down emoji means that you want this component to be excluded from the Design System.   |
| 👀 | Neutral | An eyeballs emoji communicates a neutral opinion. This means you have read the proposal and have no particular objections or support for this proposal. |

Proposals ready for voting have a `Status: Voting open` label (here’s a list).

### Adding information to an existing proposal

Often, proposals will have gaps of information. You can help advance existing proposals by adding research, context, solutions, etc., in the proposal comments. You can also open a pull request against the proposal’s branch if you have substantial changes.

Proposals that lack information will be tagged with the  `Needs: Information` label. See which proposals need help [here].

### Sharing opinions and asking questions

As a community member, your thoughts and opinions are important. If you have something to add to the conversation, we encourage you to ask questions and share your thoughts in the proposal's pull request comments. Please note that all discussions must follow our [community guidelines](https://designsystem.digital.gov/about/community/#community-conduct).

You can comment on any proposal with the `Status: Submitted` or `Status: Voting open` label. You can find a [list of all open proposals here].

## Proposal evaluation

Once complete, every proposal will enter a final comment period that lasts a minimum of [X] business days. After the voting period ends, the USWDS core team will evaluate the proposal against [this acceptance criteria]. 

Final evaluation will be led by the USWDS core team. The proposal will exit the evaluation with one of the following outcomes:

- `Accepted`: The core team determined that the proposed component is a good fit for the Design System. 
- `Accepted with notes`: The core team determined that the proposed component would be a good fit for the Design System after some amendments.
- `Hold`: The core team is interested in this addition to the Design System, but is not yet able to schedule development. A "Hold" status will accompany the "Accepted" or "Accepted with notes" status.
- `Will not pursue`: The core team decided that the proposed component is not a good fit for the Design System at this time. Reasons for denial will be included in the proposal's pull request.
- `Needs revision`: The core team decided that the proposal has not not yet made a compelling case, but believes that with improvements, it could be accepted. Proposals with this status will be sent back to the "Submitted" status and receive the "Needs: revision" label with suggestions for improvement.

## Roles and responsibilities

The USWDS core team consists of [TK] and is responsible for [TK].

Both the core team and community members will:

- Submit proposals 
- Advance existing proposals by contributing information, research, and opinions
- Vote on proposals

The USWDS core team will:

- Manage timelines
- Work with the community to ensure that all the required information has been provided
- Evaluate proposals
- Schedule the development of approved proposals
