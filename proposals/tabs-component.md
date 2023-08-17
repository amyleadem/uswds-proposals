<!---
Welcome! Thank you for contributing to the U.S. Web Design System.
Your contributions are vital to our success and we are glad you're here to share your ideas.

A few things to remember when filling out the template:
- An asterisk (*) indicates a required field.
- You must complete all required fields before your proposal can be considered for the Design System.
  However, to initially submit a proposal you must only complete [TK].
  You or someone else can finish the rest later.
- You can find full instructions for creating a proposal in the uswds-proposals repo:
  https://github.com/amyleadem/uswds-proposals/blob/add-readme-and-template/proposals/proposal-template.md

More information about contributing to USWDS can be found on the contribution page:
https://designsystem.digital.gov/about/contribute/
 -->

## About this component

### Component name

Tabs

### Description

The tabs component lets users navigate between related sections of content, displaying one section at a time.

### Problem statement

_Explain the need for this component._
- _What user need does this component address?_
- _What problem does this component solve?_
- _What gap does this component fill in the design system?_

Tabs are a familiar user pattern that allow users to stay in place

There are a few gaps that the tabs component fills:
- **Horizontal grouping of related information.** While an Accordion offers vertical grouping of disparate, unrelated content that allows more than one group of content to be opened at once, a tabs component can offer horizontal grouping.
- Offering users the ability stay in place while alternating between two or more groups of related content.
- User familiarity and expectations of a tab functionality is not present within any other component.

### Related laws or policies

N/A

### Proposed solution

_Thoroughly describe the component and how it addresses the issues outlined in the problem statement._
- [x] _Add diagrams, images, prototypes, and/or wireframes that visually demonstrate the component._
- [x] _Describe the component's core functionality. If the component is dynamic, describe its interactive states._
- [ ] _Identify any proposed variants for this component._

#### Demonstration
This is a preview of the proposed component: https://demo.badger.wwps.aws.dev/fire-safety-and-emergency-medical-services

#### States

There are three states for the tabs in this component:

##### Unselected/Inactive
The state a tab displays when it is not selected, or showing content. Here is some example code:
```CSS
.tab-style {
  @include u-text("base", "!important");
  background-color: transparent !important;
}
```

##### Selected/Active
The state displayed after a user has clicked or tapped a tab which displays only the content belonging to the tab selected. Here is some example code:
```CSS
.tab-style-active {
  @include u-text("base", "!important");
  background-color: transparent !important;
  border-bottom: 3px solid color("base-dark") !important;
}
```

##### Hover
Displayed when a user is hovering over the selection area. Here is some example code:
```CSS
.tab-style:hover {
  @include u-text("base-dark", "!important");
  background-color: transparent !important;
}
```

#### Variants
##### Tabs to the side

#### Tabs on top

### Additional context
[Tabs – Component overview.jpg.zip](https://github.com/uswds/uswds/files/8861616/Tabs.Component.overview.jpg.zip)
[Tabs – Design Demo.fig.zip](https://github.com/uswds/uswds/files/8861618/Tabs.Design.Demo.fig.zip)

### Implementation examples

 - [GOV.UK design system tabs component](https://design-system.service.gov.uk/components/tabs/)

### Related components

_Identify if this component is connected to other USWDS components._
- _Does this component require any other USWDS component to support its common interactions?_
- _Would this component affect or replace any other USWDS components?_

### Supporting evidence

_Provide links to research findings or evidence that support the need for this component._

### Alternatives

_Share any alternatives to this component and explain their advantages and disadvantages._
- _Why is this component the most effective solution?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._

## Usage

### When to use this component

- If you need to organize and group different blocks of content.
- If you are adding a small to moderate amount of content within tabs.
- If your use case involves a user needing to digest smaller amounts of information at one time, use tabs.

### When to consider a different component

- If you are organizing a large amount of disparate content.
- If you need more than one group of hidden content on a page to display at once, consider the ‘Accordion’ component instead.
- If your use case involves building a FAQ or different blocks of content that may need to be shown at one time, use the 'Accordion' component.

## Usability and accessibility

### Key usability considerations

- _What does this component need to do to be successful and effective?_
- _What are the characteristics of a successful interaction with this component?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._

#### Implementation guidance

- **Limit label to few words.** Tab labels should allude to content nested within tab as concisely as possible.
- **Allow entire tab area to be selectable** Allow users to click or tap anywhere in the label area to open a tab and view its content.
- Enable accessible horizontal scrolling in a single row to accommodate limited horizontal viewports.
- Place tabs at the top of the module or element where the content is being grouped. Fix to top of viewport as necessary.
- Do not use favicon or icons in tabs.
- Use similar punctuation between each tab.

#### Ideal component content

- In general, tabs should be paired with content-driven components like text, images, or data visualizations.
- Avoid combining tabs with other components that nest content. For instance, adding an ‘Accordion’ inside of a tab’s content should be avoided.
- Tabs should be used to group content. It is not recommended to place other highly interactive components within a tab, or components that are task-driven like forms, data entry, or page-level alerts.

#### Audiences who would benefit

- Users who have difficulty comprehending large quantities of information at once, or people with learning disorders such as dyslexia may benefit the most from tabbed content. These users will be able to select specific tabs and choose what to read without having to scan the entire content of a page at once.

### Common usability issues

- _What would make this component less usable?_
- _What are common pitfalls or implementation mistakes associated with this component?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._

- A team may mistakenly use tabs as a means of site-level navigation. Tabs should be used only for relating relative content within a page or module.
- A team may mistakenly use tabs as a means to compare content between tabs.

### Risks and potential harm

- _Are there any audiences that might struggle with this component?_
- _Are there any reasons we should not develop this component?_
- _How might this component be misused?_
- _Is this component inaccessible to any assistive technologies? (keyboard navigation, screen readers, zoom magnification, voice command, etc)_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._

- Mislabeling tabs that would cause users to miss information nested within hidden components.
- While content nested within tabs can be found in most search engine results, finding this content within a page using keyboard find functionality can prove difficult for some users. This complexity can be alleviated with an in-page search present on pages with tabs that users can use to search for content that may be behind components like an ‘accordion’ or ‘tab’.

### Accessibility considerations

- Tabbing to highlight active state
- Aria-label for screen reader to indicate each tab is a ‘tab panel’, and its name
- Aria-label indicates if currently selected is the ‘active tab panel’
- Keyboard interaction: Pressing Enter select the active, highlighted tab panel
- Arrow key tab functionality
- Hover state used as a signifier

#### Accessibility recommendations
- JAWS and NVDA users find it helpful if all expandable components like accordions and tabs announce their element type (with descriptive naming conventions that allude to the content nested inside of them) to save confusion and enable the element to be predictable, and understood.

## Stakeholders

### Key audiences

_Identify if there are any audiences that have a unique interest in this component._
- _Which audience is best able to determine if this component is successful?_

### Endorsements

_If there is significant support from a given agency or group, include their names here and tag any stakeholders._

### Volunteers
_If there are any volunteers who are willing to help design, develop, or test this component, tag them here with details about their roles._

### Contributors

Mazen Kharbutli, Software Development Engineer, AWS
Miguel Abreu, Software Development Engineer, AWS
Tanner Bachelor, User Experience Designer, AWS

### Acknowledgements

_Thank those who have helped carry out this research and work._