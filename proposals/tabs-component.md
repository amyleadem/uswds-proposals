<!--# About this component-->

## Component name
<!--
- _Does this component have a common name?_
- _Are there other existing names for this component?_
-->
Tabs

## Description
<!-- _Provide a one-sentence description of the component._ -->

Tabs allow users to navigate through individual sections of related content without changing location on the page. 

## Motivation
<!--
_Explain the need for this component._
- _What user need does this component address? What audiences would benefit from this component?_
- _What gap does this component fill in the Design System? How is this different from existing USWDS components?_
- _What problem does this component solve?_
-->
### How would this component help end users?
Tabs are a familiar user pattern that lets users progressively show and hide digestible sections of content while staying in place on a page. 

#### Audiences who would benefit
Users who have difficulty comprehending large quantities of information at once, or people with learning disorders such as dyslexia may benefit the most from tabbed content. These users will be able to select specific tabs and choose what to read without having to scan the entire content of a page at once. [Needs source/research]

### What gap does this fill in the Design System?
USWDS offers an accordion component, which also gives users the ability to show and hide groups of content. However tabs would address the following gaps that the accordion doesn't cover:

- **Tabs allow for horizontal grouping of information.** While the accordion offers vertical grouping of content that allows more than one group of content to be opened at once, a tabs component can offer horizontal grouping.
- **Tabs allow users to navigate through similarly structured content.** One feature of tabs is that it allows users to move between content and quickly see similarities/differences.  
- **Tabs allow users to stay in place while navigating sections of content**. Unlike accordion, tabs offers users the ability stay in place while alternating between two or more groups of related content.

### How would this component help teams?
Tabs are a a very common and familiar user pattern that are used on a range of existing digital experiences. Jakob’s Law of UX states: “Users spend most of their time on other sites. This means that users prefer your site to work the same way as all the other sites they already know.” Offering a USWDS tabs component would provide the following benefits:

- **Providing a common tabs component will save time and money across projects.** Because tabs is such a familiar and in-demand component,  federal agencies are spending time designing, building, and testing custom implementations of the tabs component. Development could be streamlined by introducing a USWDS implementation. 
- **USWDS can provide guidance for this common pattern.** Additionally, USWDS will be able to provide guidance on when builders should use tabs, when to consider something else, and additional support by including a component overview page as seen with other components within the library. To help facilitate the introduction of this tabs component, we have included a draft of what may be included in a tabs overview page in this proposal. (See Tabs – Component overview.jpg.zip).

## Related laws or policies
<!-- _Share if there are there are any laws or policies that this component directly supports._-->
N/A

## Proposed design
<!--
_Thoroughly describe the component and how it addresses the issues outlined in the problem statement._
- _Add diagrams, images, and/or wireframes that visually demonstrate the component._
- _Describe the component's core functionality. If the component is dynamic, describe its interactive states._
- _Identify any proposed variants for this component._
-->

### Demonstration
The constructed design file can be found in the following file: [Tabs – Design Demo.fig.zip](https://github.com/uswds/uswds/files/8861618/Tabs.Design.Demo.fig.zip).

To preview the tabs component live in any browser, visit: https://demo.badger.wwps.aws.dev/fire-safety-and-emergency-medical-services.

### Implementation examples
<!-- _Provide a list of examples of this component on government (preferred) or non-government sites._-->
- [GOV.UK design system tabs component](https://design-system.service.gov.uk/components/tabs/)
- [State.gov home page](https://www.state.gov/)

### Core functionality
- Tabs should contain at least two items
- Users should be able to activate only one tab at a time one
- Tabs should be navigable by click, keyboard, and voice command
- Tabs should horizontally scroll to prevent content from being cut off
  
### Possible variants
- Tabs to the side 
- Tabs on top
- Scrollable

### Component code
```html
<div
  role="tab"
  class="tab-style display-inline-block padding-x-2 padding-y-105
         text-bold font-sans-md"
  tabindex="0"
  aria-label="Active Section Tab label" 
  style="cursor: pointer; white-space: nowrap;"
>
Tab label
</div>
```

### States

The tab-style css class has three states:

#### Unselected/Inactive
The state a tab displays when it is not selected, or showing content. 
<details>
  <summary>Sample code</summary>
```CSS
.tab-style {
  @include u-text("base", "!important");
  background-color: transparent !important;
}
```
</details>

#### Selected/Active
The state displayed after a user has clicked or tapped a tab which displays only the content belonging to the tab selected.
<details>
  <summary>Sample code</summary>
  ```CSS
  .tab-style-active {
    @include u-text("base", "!important");
    background-color: transparent !important;
    border-bottom: 3px solid color("base-dark") !important;
  }
  ```
</details>

#### Hover
Displayed when a user is hovering over the selection area. 
<details>
  <summary>Sample code</summary>
  ```CSS
  .tab-style:hover {
    @include u-text("base-dark", "!important");
    background-color: transparent !important;
  }
  ```
</details>

## Related components
<!--_Identify if this component is connected to other USWDS components._
- _Does this component require any other USWDS component to support its common interactions?_
- _Would this component affect or replace any other USWDS components?_-->
N/A

<!--## Supporting evidence

_Provide links to research findings or evidence that support the need for this component._

## Alternatives

_Share any alternatives to this component and explain their advantages and disadvantages._
- _Why is this component the most effective solution?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._-->

## Usage

### When to use this component
<!--_Define the appropriate use case for this component._
- _What common patterns or interactions does this component support?_-->
- **If you want to group together two or more sections of related information.**
- **If your users would benefit from digesting smaller amounts of information at a time.**
- **If your sections do not have lengthy or complex content.**

- More information can be found in the [Tabs – Component overview.jpg.zip](https://github.com/uswds/uswds/files/8861616/Tabs.Component.overview.jpg.zip)

### When to consider a different component
- **If you are organizing a large amount of unrelated content.** 
- **If you need site navigation.** Avoid using tabs as navigation to other pages. Instead, use the header component.
- **If you need to show more than one hidden section at a time.** Instead, use the accordion component.
- **If more than three tabs are needed.** Consider using an accordion when more than a few tabs will be required. This eliminates the need for horizontal scrolling, which can lead to a poor experience for uses of assistive technologies.
- **If you need more than one group of hidden content on a page.** In this scenario, consider the accordion component instead.

#### Implementation guidance

- **Provide informative tab labels.**
- **Be strategic when grouping content.** Only use tabs that are similar when it comes to the meaning of the page.
- **Limit label to few words.** Tab labels should allude to content nested within tab as concisely as possible.
- **Allow entire tab area to be selectable** Allow users to click or tap anywhere in the label area to open a tab and view its content.
- **Enable horizontal scrolling.** This allows content to be accessible in limited horizontal viewports.
- **Use similar punctuation between each tab.**
- **Do not use favicon or icons in tabs.** 
- **Do not use all caps for tabs labels.** Using caps will shorten your available horizontal space and will demand too much attention from the user.
- **Place tabs at the top of the module or element where the content is being grouped.** Fix to top of viewport as necessary.
- **If the number of content items inside a tab is relevant, indicate the number with parentheses.** If tabs are being used to display contnet that is grouped into numerical data sets, it may be helpful to indicate to the user the number of data sets within each tab.

#### Ideal component content
- In general, tabs should be paired with content-driven components like text, images, or data visualizations.
- Avoid combining tabs with other components that nest content. For instance, adding an ‘Accordion’ inside of a tab’s content should be avoided.
- Tabs should be used to group content. It is not recommended to place other highly interactive components within a tab, or components that are task-driven like forms, data entry, or page-level alerts.
  
### Accessibility guidance
- **Preserve visual tab order.** Tabs should read out in the order they appear in the visual layout.
- **Label when the tab content is active.** Use an `aria-label` to indicate when the content is selected. 
- Tabbing to highlight active state
- Aria-label for screen reader to indicate each tab is a ‘tab panel’, and its name
- Keyboard interaction: Pressing Enter select the active, highlighted tab panel
- Arrow key tab functionality
- Hover state used as a signifier
  
<!--### Key usability considerations

- _What does this component need to do to be successful and effective?_
- _What are the characteristics of a successful interaction with this component?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._
-->


<!--
### Common usability issues
- _What would make this component less usable?_
- _What are common pitfalls or implementation mistakes associated with this component?_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._
-->

### Risks and potential harm
<!--
- _Are there any audiences that might struggle with this component?_
- _Are there any reasons we should not develop this component?_
- _How might this component be misused?_
- _Is this component inaccessible to any assistive technologies? (keyboard navigation, screen readers, zoom magnification, voice command, etc)_
- _When possible, provide supporting links to research findings or supporting evidence (your own, or other available research)._-->
- **A team may mistakenly use tabs as a means of site-level navigation.** Tabs should be used only for relating relative content within a page or module.
- **Users might not find content inside of tabs.** Tabs hide content from users, which introduces the risk that users might not notice or read all of the included content.
- **Tabs add an extra click.** If you know your users will want to see the content, don't hide it behind a tab.
- A team may mistakenly use tabs as a means to compare content between tabs.
- **Hiding content can cause users to miss nested information.**
- **Searching for content can be difficult.** While content nested within tabs can be found in most search engine results, finding this content within a page using keyboard find functionality can prove difficult for some users. This complexity can be alleviated with an in-page search present on pages with tabs that users can use to search for content that may be behind components like an ‘accordion’ or ‘tab’.

### Accessibility considerations
- In a reimagined experience on va.gov, a veteran relying only on their keyboard will be able to use tabs to compare their healthcare overview from 2022 to the previous year the same way a mouse and keyboard user would.
- A farmer in rural Ohio who relies on a screen magnifier and a screen reader can identify the farm loan program they are looking for which has been labeled by tabs and are properly displayed and functional when zoomed in at 400%, and read by a screen reader.

- For low-vision users who require a zoom up to 400%, some tabs would appear off-screen even at large viewports, rendering the component unusable. To address this, we implemented a horizontal scroll and ultimately wrapped tab items in divs top to bottom to provide an experience that was more consistent than what we were able to achieve using list items within lists.

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

- Mazen Kharbutli, Software Development Engineer, AWS
- Miguel Abreu, Software Development Engineer, AWS
- Tanner Bachelor, User Experience Designer, AWS

### Acknowledgements

_Thank those who have helped carry out this research and work._
