# QHO542 Human Computer Interaction

# Week 7 Seminar Challenge

## Interface Forensics, Wireframing and Technical UX Redesign

---

# Seminar Challenge

Today you are not simply going to create a wireframe.

You will work like a **UX/Product Engineering team**.

Your job is to:

```text
Investigate an existing interface
        ↓
Understand how the interface works
        ↓
Identify the user journey
        ↓
Measure the difficulty of completing the task
        ↓
Identify technical UX problems
        ↓
Sketch alternative solutions
        ↓
Create a better wireframe
        ↓
Test whether your redesign is actually better
```

---

# What You Will Learn

By the end of this seminar you should be able to:

* analyse an existing digital interface
* identify its information architecture
* identify the main user flow
* break a task into individual steps
* identify usability and accessibility problems
* understand interface states such as loading, error and success
* understand how technical performance affects UX
* sketch several possible solutions quickly
* produce a low-fidelity wireframe
* justify a redesign using HCI evidence

---

# The Main Idea

A user interface is NOT simply a collection of screens.

A real interface contains:

```text
Users
Tasks
Navigation
Information
Decisions
System states
Errors
Feedback
Accessibility
Performance
Responsive behaviour
```

This week you will investigate all of these.

---

# Your Scenario

You are part of a product team reviewing an existing digital product.

Your team has been asked to improve **one important user journey**.

Examples:

```text
Finding accommodation

Ordering food

Booking an appointment

Finding university information

Registering for an event

Searching for a product

Submitting an enquiry

Finding support

Completing a checkout

Logging into a service
```

You must investigate the current experience before redesigning it.

---

# Team Setup

Work in teams of approximately 3–4 students.

Suggested roles:

```text
UX Researcher
Investigates the user journey and usability issues.

Technical Investigator
Uses browser tools to inspect the interface.

UX Designer
Creates sketches and wireframes.

Accessibility / Testing Lead
Checks accessibility and tests the final journey.
```

You may rotate roles during the activity.

---

# Choose Your Interface

Choose ONE public website or digital service.

Examples:

* GOV.UK
* Airbnb
* Booking.com
* Amazon
* Spotify
* GitHub
* university website
* restaurant website
* hotel website
* e-commerce website
* learning platform

Do not choose a website where completing the task requires making a real payment.

---

# PART 1 — Define the User and Task

## Time: 10 minutes

Before touching the design, define the user.

Complete:

```text
Website:

Main user:

Main user goal:

Device:

Context:

Main task:

Expected final outcome:
```

---

## Example

```text
Website:
Hotel booking website

Main user:
A visitor looking for accommodation

Main user goal:
Find a hotel within budget

Device:
Mobile phone

Context:
Searching while travelling

Main task:
Search → Compare → Select hotel

Expected outcome:
User identifies a suitable hotel
```

---

# HINT

Do not write:

```text
Goal: Use the website
```

That is too vague.

Write something measurable:

```text
Goal:
Find accommodation in London for two people under £150.
```

---

# PART 2 — Interface Forensics

## Time: 15 minutes

Now investigate the current interface.

Do NOT redesign anything yet.

Open the website and identify:

```text
Navigation

Main content

Buttons

Forms

Search

Filters

Images

Calls to action

Feedback messages

Footer

Important information
```

Record what you observe.

---

## Questions

Answer:

1. What does your eye notice first?
2. What is the primary action?
3. Is that action obvious?
4. What information is most important?
5. Is related information grouped?
6. Can you immediately understand the navigation?
7. What information appears unnecessary?
8. What may confuse a first-time user?

---

# HINT

Remember previous HCI concepts:

```text
Visual hierarchy

Gestalt principles

Proximity

Similarity

Common region

Consistency

Affordance

Feedback

Cognitive load
```

Do not simply write:

```text
"The website looks bad."
```

Explain WHY.

Better:

```text
The booking button competes visually with several other buttons,
making the primary action difficult to identify.
```

---

# PART 3 — Technical Interface Investigation

## Time: 15 minutes

Open:

```text
Browser
→ Developer Tools
→ Elements / Inspector
```

You are NOT expected to understand every line of code.

Your goal is to understand how UI design decisions connect to the underlying HTML.

Look for:

```html
<header>
<nav>
<main>
<section>
<button>
<form>
<input>
<img>
<footer>
```

---

# Task

Find at least:

```text
1 navigation element

1 button

1 image

1 form/input if available

1 heading
```

Record the HTML element being used.

---

## Example

You may find:

```html
<button>Book Now</button>
```

or something like:

```html
<div class="button">Book Now</div>
```

Ask yourself:

Which one better communicates that this is an interactive control?

---

# HINT

Semantic HTML helps:

```text
Accessibility

Keyboard navigation

Screen readers

Search engines

Maintainability

User interaction
```

You are connecting **front-end implementation with HCI**.

---

# PART 4 — Keyboard-Only Challenge

## Time: 10 minutes

Now stop using your mouse.

Try to complete the main task using only:

```text
TAB
SHIFT + TAB
ENTER
SPACE
ARROW KEYS
ESC
```

Record:

```text
Task completed? YES / NO

Number of TAB presses:

Was keyboard focus visible?

Did you get stuck?

Was the navigation order logical?

Could you activate the important controls?
```

---

# Important

Do not worry if the website performs badly.

That is useful evidence.

---

# Discussion

Ask:

```text
Could somebody who cannot use a mouse complete this task?
```

If the answer is no, you have discovered an accessibility problem.

---

# PART 5 — Measure the User Journey

## Time: 10 minutes

Now complete the task normally.

Count what happens.

Use this table:

| Measure               | Result |
| --------------------- | ------ |
| Screens/pages visited |        |
| Clicks required       |        |
| Decisions required    |        |
| Form fields completed |        |
| Scrolls               |        |
| Backtracks            |        |
| Errors/confusion      |        |
| Approximate task time |        |

---

# Interaction Cost

Think of interaction cost as:

```text
Interaction Cost =
Physical Effort
+
Mental Effort
+
Time
```

---

# Questions

Where is interaction cost highest?

Why?

Could any step be removed?

Does the user need to remember information between screens?

Does the user make unnecessary decisions?

---

# HINT

Every additional step is not automatically bad.

A step is bad when it adds effort **without helping the user**.

---

# PART 6 — Reconstruct the User Flow

## Time: 15 minutes

Now draw the journey.

You can use:

* paper
* FigJam
* Figma
* diagrams.net
* Miro
* any diagramming tool approved by your tutor

Example:

```text
START
  ↓
Homepage
  ↓
Search
  ↓
Results
  ↓
Apply filters
  ↓
Select item
  ↓
View details
  ↓
Complete task
  ↓
END
```

---

# Add Decision Points

Real flows contain decisions.

Example:

```text
Search
  ↓
Are results available?
  ↓
 ┌─────────────┐
 YES           NO
 ↓              ↓
Results      Empty State
 ↓              ↓
Continue       Search Again
```

Your flow must contain:

```text
Start

At least 5 steps

At least 1 decision

At least 1 alternative path

Final task completion
```

---

# PART 7 — Find the Invisible States

## Time: 10 minutes

Most beginner designs only create the normal screen.

Real applications must handle many states.

Find or imagine how your chosen interface should handle:

```text
Loading

Empty

Success

Error

Invalid input

Disabled

Offline

No results
```

Choose at least FOUR.

Complete:

```text
STATE 1:

What is happening?

What should the user see?

What action should the user take?
```

---

## Example

```text
State:
No search results

What happened:
The user's filters returned no matching hotels.

Bad experience:
Blank page.

Better experience:
"No hotels match these filters."

Suggested actions:
Clear filters
Change dates
Increase distance
Change price range
```

---

# HINT

A good interface should answer:

```text
What happened?

Why did it happen?

What can I do next?
```

---

# PART 8 — Error Prevention vs Error Recovery

## Time: 10 minutes

Identify ONE place where the user could make a mistake.

Example:

```text
Invalid email

Incorrect date

Missing required information

Wrong search query

Unavailable item

Invalid password
```

Now design TWO solutions.

---

## Error Prevention

Stop the problem before it happens.

Example:

```text
Select a date from the calendar.
Past dates are disabled.
```

---

## Error Recovery

Help after something goes wrong.

Example:

```text
"This date is unavailable.
Please choose another date."
```

---

# Question

Which approach creates the better experience?

Sometimes both are required.

---

# PART 9 — Performance Is UX

## Time: 10 minutes

Open:

```text
Developer Tools
→ Network
```

Reload the website.

Observe:

```text
How quickly does content appear?

Do images appear slowly?

Does the page move while loading?

Does the user wait before interacting?

Are loading indicators shown?
```

If available, use Network Throttling to simulate a slower connection.

---

# Think

Imagine the user is:

```text
Travelling

Using public Wi-Fi

Using mobile data

Using an older device
```

Does the experience remain usable?

---

# Important Concept

```text
Technical Performance
        ↓
User Perception
        ↓
User Experience
```

A visually excellent website can still provide poor UX if it is extremely slow.

---

# PART 10 — Responsive Investigation

## Time: 10 minutes

Open:

```text
Developer Tools
→ Device Toolbar / Responsive Mode
```

Compare approximately:

```text
Small mobile

Tablet

Desktop
```

Observe:

```text
Navigation

Buttons

Images

Text

Spacing

Forms

Content priority
```

---

# Questions

What disappears?

What moves?

What becomes collapsed?

Does navigation change?

Do buttons remain easy to select?

Does important information stay visible?

---

# HINT

Responsive design does NOT mean:

```text
Make everything smaller.
```

It means deciding how the experience should change depending on the device.

---

# PART 11 — Crazy 8 Sketching Challenge

## Time: 10 minutes

Now you may redesign.

But first:

NO Figma.

NO AI.

Take a sheet of paper.

Divide it into eight sections.

Create:

```text
8 ideas
in
8 minutes
```

Each idea should solve the main user problem in a slightly different way.

---

# Rules

Do not focus on:

```text
Colours

Perfect icons

Fonts

Beautiful graphics
```

Focus on:

```text
Navigation

Information

Buttons

Hierarchy

Task completion

Feedback
```

---

# HINT

Bad approach:

```text
Idea 1
↓
Spend 8 minutes making it beautiful
```

Correct approach:

```text
Idea 1
Idea 2
Idea 3
Idea 4
Idea 5
Idea 6
Idea 7
Idea 8

↓

Compare

↓

Select
```

---

# PART 12 — Select the Best Concept

## Time: 5 minutes

Place all sketches together.

Each team member gets THREE votes.

Vote for:

```text
Best navigation

Best interaction

Best information organisation
```

Combine the strongest ideas.

Do not automatically select the prettiest sketch.

---

# PART 13 — Create the Improved User Flow

## Time: 10 minutes

Now redesign the original flow.

Original:

```text
A → B → C → D → E → F
```

Can you improve it?

Maybe:

```text
A → B → C → D
```

But shorter is not always automatically better.

Your redesigned flow should reduce:

```text
Unnecessary actions

Confusion

Backtracking

Memory requirements

Repeated information

Unclear decisions
```

---

# PART 14 — Build the Wireframe

## Time: 20 minutes

Create approximately:

```text
2–3 connected screens
```

You may use:

```text
Figma

FigJam

Penpot

Paper

Another approved wireframing tool
```

---

# Important Rule

Your wireframe should initially be LOW FIDELITY.

Use:

```text
Boxes

Lines

Basic text

Buttons

Image placeholders

Simple forms
```

Avoid spending time on colour or branding.

---

# Your Design Must Demonstrate

At least:

```text
Clear visual hierarchy

Logical information architecture

Clear primary action

Consistent navigation

Accessibility consideration

Feedback

Error handling

Responsive thinking
```

---

# PART 15 — Technical Constraint Challenge

Your redesign must satisfy ALL of the following.

## Constraint 1

The primary user task should ideally require no more than approximately:

```text
5 major interactions
```

Explain if more are necessary.

---

## Constraint 2

Your design must work conceptually on:

```text
Mobile

Desktop
```

---

## Constraint 3

Important functionality must be keyboard accessible.

---

## Constraint 4

You must design these states:

```text
Normal

Loading

Error

Success
```

---

## Constraint 5

Your interface must provide feedback after important actions.

Examples:

```text
Saving...

Booking confirmed

Search completed

Form error

Item unavailable
```

---

# PART 16 — Prototype Testing

## Time: 10 minutes

Give your design to another team.

Do NOT explain how the interface works.

Give them only a task.

Example:

```text
"You need to find accommodation in London for two people.
Show us how you would do it."
```

Observe silently.

Record:

```text
Task completed?

Number of interactions:

Wrong clicks:

Hesitations:

Unexpected behaviour:

Questions asked:

Where did the user get stuck?
```

---

# IMPORTANT

Do NOT help the participant.

If you explain where they should click, you are testing your explanation, not your interface.

---

# PART 17 — Evidence-Based Iteration

Now change ONE thing based on the test.

Use:

```text
Finding:

Evidence:

Interpretation:

Change:
```

---

## Example

```text
Finding:
Users struggled to find the booking action.

Evidence:
3 users opened the Contact page before seeing Book Now.

Interpretation:
The primary call-to-action does not have enough visual priority.

Change:
Move Book Now into the main navigation and increase its visual prominence.
```

---

# Do NOT Write

```text
Users didn't like the website.
```

Write something observable.

---

# FINAL DELIVERABLE

Your group should finish the seminar with:

```text
1. User and task definition

2. Original interface observations

3. Technical HTML/accessibility observation

4. Keyboard-navigation result

5. Interaction-cost measurements

6. Original user flow

7. Four interface states

8. Error prevention/recovery example

9. Performance observation

10. Responsive observation

11. Crazy 8 sketches

12. Improved user flow

13. 2–3 screen wireframe

14. Usability test result

15. One evidence-based redesign
```

---

# FINAL PRESENTATION

Each group has approximately 3 minutes.

Do NOT explain every screen.

Present the investigation.

---

## Slide / Section 1 — The Problem

```text
Our user:

Their goal:

The interface:

The task:
```

---

## Slide / Section 2 — Evidence

Show something measurable.

Example:

```text
Original journey:

7 screens

9 clicks

14 keyboard actions

2 confusing decisions

1 accessibility issue
```

---

## Slide / Section 3 — Technical Issue

Examples:

```text
Poor semantic structure

Keyboard issue

No visible focus

Missing feedback

Poor error state

High interaction cost

Poor responsive behaviour

Slow-loading content
```

---

## Slide / Section 4 — Redesigned Journey

Show:

```text
BEFORE

A → B → C → D → E → F


AFTER

A → B → C → D
```

Explain WHY it is better.

---

## Slide / Section 5 — Test Result

Example:

```text
Before:
Users struggled to identify the main action.

After:
Test participant immediately identified the primary CTA.
```

---

# OPTIONAL ADVANCED CHALLENGE

If you have development experience, implement one part of your design using:

```text
HTML
CSS
JavaScript
```

Your prototype should include multiple application states.

Example:

```javascript
const state = "loading";

if (state === "loading") {
    // Show loading UI
}

if (state === "error") {
    // Show error and recovery option
}

if (state === "success") {
    // Show completed result
}
```

Think about the relationship:

```text
Application Logic
       ↓
Application State
       ↓
Interface State
       ↓
User Experience
```

---

# OPTIONAL JSON CHALLENGE

Imagine the system receives:

```json
{
  "hotels": [
    {
      "id": 1,
      "name": "London Central Hotel",
      "price": 120,
      "available": true
    },
    {
      "id": 2,
      "name": "City Stay",
      "price": 145,
      "available": false
    }
  ]
}
```

Your interface must decide what to display.

Possible states:

```text
Loading data
     ↓
Data received?
   ↙       ↘
 YES       NO
 ↓          ↓
Check       Error
results
 ↓
Any results?
 ↙       ↘
NO        YES
↓          ↓
Empty     Display
State     Results
```

This is an example of how **software logic and HCI connect**.

---

# HINTS

## Hint 1

Do not redesign too early.

First understand:

```text
What is happening?

Who is using it?

Why are they struggling?
```

---

## Hint 2

Do not evaluate only appearance.

A technically weak interface can still look attractive.

Look at:

```text
Task completion

Accessibility

Feedback

Errors

Performance

Navigation

States

Cognitive effort
```

---

## Hint 3

Always ask:

```text
Can I remove this step?
```

Then ask:

```text
Would removing it create another problem?
```

---

## Hint 4

Think about users who are:

```text
In a hurry

Using mobile data

Using one hand

Using keyboard only

Using screen readers

New to the service

Not confident with technology
```

---

## Hint 5

Every important action needs feedback.

If a user presses:

```text
Submit
```

something should tell them:

```text
Submitting...

Success

OR

Something went wrong
```

Never leave the user wondering.

---

## Hint 6

Design failure as carefully as success.

Real applications do not always work perfectly.

Ask:

```text
What if the network fails?

What if no results exist?

What if input is incorrect?

What if the user changes their mind?

What if the system is slow?
```

---

# INDUSTRY CONNECTION

Modern UX/Product teams commonly work across:

```text
UX Research
        ↓
Task Analysis
        ↓
Information Architecture
        ↓
User Flow
        ↓
Sketching
        ↓
Wireframing
        ↓
Prototype
        ↓
Usability Testing
        ↓
Engineering
        ↓
Analytics
        ↓
Iteration
```

The important skill is therefore NOT:

```text
"Can I use Figma?"
```

It is:

```text
Can I identify a user problem?

Can I produce multiple solutions?

Can I justify one?

Can I test it?

Can I interpret evidence?

Can I improve the design?
```

---

# KEY WEEK 7 MESSAGE

```text
A UI is not a picture.

It is an interactive system containing:

States
Transitions
Decisions
Errors
Feedback
Accessibility
Performance
User behaviour
```

---

# FINAL CHALLENGE

Before finishing, your group should be able to answer:

```text
Who is our user?

What are they trying to achieve?

What does the current journey look like?

Where is the highest interaction cost?

What accessibility problem exists?

What happens when the system fails?

What did we change?

What evidence supports the change?

Did testing show an improvement?
```

If you cannot answer one of these questions, investigate further.

---

# Final Rule

Do not say:

> "We redesigned it because it looks better."

Say:

> "We redesigned it because our investigation identified a specific usability problem, and our new design reduces the effort required to complete the task."

That is the difference between simply making screens and practising Human Computer Interaction.
