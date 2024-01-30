# USWDS proposals

This repo acts as a public hub to submit and discuss proposals for new U.S. Web Design System (USWDS) components.

> [!Important]
> At this time, we are accepting proposals only for new components.
>
> You can submit requests for new features or enhancements by [creating an issue](https://github.com/uswds/uswds/issues/new/choose) in the uswds repo.

## Overview of the proposal process

**All requests for new USWDS components must be submitted as a proposal.** Proposals are detailed documents that should make a compelling case for adding a new component to the design system.

**Anyone can submit or contribute to a proposal.** Community contribution is at the heart of this process, and we encourage you to share your ideas, opinions, and votes.

### Ways to contribute

The proposal process helps the USWDS team understand community interest in new components. Your opinions matter, and we want to make it easy for you to contribute.

The resources in this repo can guide you through the process:

- [Instructions for submitting a new proposal](#submitting-a-new-proposal)
- [Instructions for contributing to an existing proposal](#contributing-to-an-existing-proposal)
- [Information about our evaluation process](#proposal-evaluation)
- [Information about roles and responsibilities](#roles-and-responsibilities)
- [A proposal template](https://github.com/amyleadem/uswds-proposals/blob/main/proposals/_proposal-template.md)

#### Help with GitHub

This process requires a knowledge of GitHub [branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches) and [pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests). If you need help submitting or contributing to a proposal, please reach out via [TK].

## Submitting a new proposal

When you are ready to suggest a new USWDS component, you'll need to submit a proposal. Our proposal template guides you through the process.

You should know two things when filling out the proposal template:

- **It’s okay to start with the basics.** We understand that you’re busy and might not have the specialized resources to thoroughly fill out every section of the proposal template. Submitting your idea and explaining its benefits is a great start! An incomplete proposal gets the conversation started and creates a central location to gather ideas and feedback from the community. The USWDS team will add a “Needs: Information” tag to the proposal to encourage community participation.
- **Only complete proposals can be considered for inclusion in the Design System.** A complete proposal should make a detailed, compelling case for the new component. Every section should be filled out. If a proposal is lacking critical information, it will be sent back for revision.

### How to create and submit a new proposal

1. **First, find out if a proposal for your idea already exists.** Start by looking at the pull requests in this repo. If a proposal for your idea already exists, that’s great! You can contribute to the conversation by adding comments, adding information, and voting. Learn more about how to contribute to an existing proposal in the next section.
1. **If a proposal doesn't exist, it's time to create one.** Here are the steps:
    1. **Create a new branch.** [Create a new branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) for your proposal named: `component-[proposed component name]`. For example, if you wanted to propose adding a loader component, you would name the branch `component-loader`.
    1. **Create a new proposal file.** In your new branch, create a file in the `/proposals` directory called `component-[component name].md`. For example, `component-loader.md`.
    1. **Copy the proposal template.** Copy the contents of `proposal-template.md` into this file.
    1. **Fill out the template to the best of your ability.**  An asterisk (*) in the template indicates a required field. All required fields must be complete before your proposal can be considered for USWDS. However, you may start by submitting just the “Name”, “Description” and “Design system need” sections. You or someone else can finish the rest later.
    1. **Open a pull request.** [Open a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) (PR) with the title: `Proposal: [Component name]`. For example, `Proposal: Loader component`. Once your PR is open, it will receive a "Status: Submitted" label and will be available for voting, comments, and additions.
1. **Get the conversation started.** Once your proposal has been opened for voting, invite others to participate in the discussion and help polish the proposal. Use the [uswds-public Slack channel](https://gsa-tts.slack.com/archives/C3F14AHSQ) or reach out to peers to get feedback and support.

## Contributing to an existing proposal

Every proposal can benefit from community input. If you would like to help with existing proposals, we encourage you to contribute by:

1. [Voting for proposals](#voting-for-a-proposal)
2. [Adding information, research, and solutions](#adding-information-to-an-existing-proposal)
3. [Sharing ideas and asking questions](#sharing-opinions-and-asking-questions)

### Voting for a proposal

One of the easiest and most effective ways to express your opinion about an idea is to vote. Votes on a proposal show the community's level of interest in an idea. A proposal with many votes is more likely to be reviewed by the USWDS core team.

To vote for a proposal, add an emoji to the proposal's PR description by clicking on the smiley face at the bottom left of the description box. Here’s what each emoji means:

| Emoji            | Action | Description |
| :----------------------------: | :-------------- | :--------- |
| 👍 | Up-vote | A thumbs-up emoji means that you support including this component in the design system. |
| 👎 | Down-vote | A thumbs-down emoji means that you don’t want the component in the design system. |
| 👀 | Neutral | An eyeballs emoji communicates a neutral opinion. You have read the proposal and have no particular objections or support for the proposal. |

Proposals ready for voting have a `Status: Voting open` label (here’s a list).

### Adding information to an existing proposal

You can advance existing proposals by adding research, context, solutions, etc., in the proposal comments. You can also open a pull request against the proposal’s branch if you have substantial changes.

Incomplete proposals will be tagged with the  `Needs: Information` label. [See which proposals need help].

### Sharing opinions and asking questions

We encourage you to ask questions and share your thoughts in the proposal's pull request comments. The community’s thoughts and opinions play a critical role  in the proposal process. Please note that all discussions must follow our [community guidelines](https://designsystem.digital.gov/about/community/#community-conduct).

You can comment on any proposal with the `Status: Submitted` or `Status: Voting open` label. [See the list of open proposals].

## Proposal evaluation

Once complete, every proposal enters a final comment period that lasts a minimum of [X] business days. After the voting period ends, the USWDS core team will evaluate the proposal against [this acceptance criteria].

Final evaluation is led by the USWDS core team. The proposal will exit the evaluation with one of the following outcomes:

- `Accepted`: The proposed component is a good fit for the Design System.
- `Accepted with notes`: The proposed component would be a good fit for the design system after some revisions.
- `Hold`: The proposal is a good fit for the design system, but we are not yet able to schedule development. A "Hold" status would accompany the "Accepted" or "Accepted with notes" status.
- `Will not pursue`: The proposed component is not a good fit for the design system at this time. Reasons for the decision  will be included in the proposal's pull request.
- `Needs revision`: The proposal has not not yet made a compelling case, but with improvements it could be accepted. Proposals with this status will be sent back to the "Submitted" status and receive the "Needs: revision" label with suggestions for improvement.

## Roles and responsibilities

The USWDS core team consists of [TK] and is responsible for [TK].

Both the core team and community members will:

- Submit proposals
- Advance existing proposals by contributing information, research, and opinions
- Vote on proposals

The USWDS core team will:

- Manage timelines
- Work with the community to ensure that proposals include all the required information
- Evaluate proposals
- Schedule the development of approved proposals
