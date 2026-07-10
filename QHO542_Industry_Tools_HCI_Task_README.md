# QHO542 HCI Seminar Task  
## Industry Tools Workshop: Investigate, Analyse, Redesign and Test a Website

## Seminar Theme

In this seminar, you will work like a small digital product team.

Your goal is to investigate a real website using modern industry tools, identify user experience, accessibility, performance and technical issues, then redesign one part of the website and prepare a user feedback plan.

This task is designed to help you understand how modern HCI work is done in practice. In industry, teams do not only discuss design theory. They use tools, collect evidence, test assumptions and improve designs based on findings.

---

## Main Learning Goal

By the end of this task, you should understand how to use modern tools to support HCI decision-making.

You will use tools for:

- technical observation
- research and note organisation
- performance testing
- accessibility checking
- UX/design review
- wireframing or redesign
- questionnaire creation
- final recommendation writing

---

## Industry Tools You Can Use

You do not need to use every tool. Your group should use at least 4 tools from the list below.

### Technical Observation Tools

| Tool | Purpose |
|---|---|
| Wireshark | Observe network traffic when a website loads |
| Chrome DevTools | Inspect performance, console, network and page behaviour |
| Lighthouse | Check performance, accessibility, SEO and best practices |
| curl / ping / traceroute | Basic command-line website and network checks |

### Research and Documentation Tools

| Tool | Purpose |
|---|---|
| NotebookLM | Organise notes, summarise findings, generate checklists |
| ChatGPT / Gemini | Help explain technical terms and draft structured findings |
| Google Docs / Microsoft Word | Write your short report |
| Notion | Organise research and task notes |

### UI / UX Design Tools

| Tool | Purpose |
|---|---|
| Figma | Wireframing, UI design and prototyping |
| FigJam | Brainstorming, user journeys and collaborative mapping |
| Stitch | AI-generated UI design starting point |
| Uizard | AI-assisted wireframes and mockups |
| Canva | Simple layout and visual design |
| Penpot | Open-source design and prototyping |
| Pen and paper | Fast low-fidelity sketching |

### Accessibility Testing Tools

| Tool | Purpose |
|---|---|
| WAVE Accessibility Checker | Check accessibility errors and warnings |
| axe DevTools | Accessibility testing in browser |
| Lighthouse Accessibility | Basic accessibility audit |
| Colour Contrast Checker | Test text/background contrast |
| NVDA / VoiceOver | Screen reader testing |

### User Behaviour and Usability Tools

| Tool | Purpose |
|---|---|
| Microsoft Clarity | Heatmaps and session recording concepts |
| Hotjar | Heatmaps and behaviour analytics concepts |
| Maze | Prototype usability testing |
| Useberry | User testing and click testing |
| Google Forms | Questionnaire creation |
| Microsoft Forms | Questionnaire creation |

---

## Group Setup

Work in groups of 4 to 5.

Assign roles within your group:

| Role | Responsibility |
|---|---|
| Research Lead | Understands the website and records observations |
| Technical Lead | Uses Wireshark, DevTools or Lighthouse |
| UX Lead | Reviews layout, navigation and usability |
| Accessibility Lead | Checks contrast, labels, alt text and inclusive design |
| Design Lead | Creates the redesign sketch or wireframe |
| Presenter | Summarises and presents the final findings |

If your group has fewer students, one person can take more than one role.

---

## Website Selection

Choose one public website to investigate.

Recommended options:

- restaurant website
- university website
- portfolio website
- news website
- e-commerce website
- learning platform
- booking website
- charity website
- assessment-related website

Choose a website where users need to complete a clear task.

Examples:

| Website Type | User Task |
|---|---|
| Restaurant | Find menu, prices and contact details |
| University | Find course information |
| E-commerce | Find product and add to basket |
| News | Find latest article |
| Portfolio | Find projects and contact details |
| Learning platform | Find a lesson or resource |
| Booking website | Search and complete a booking journey |

---

## Final Deliverable

By the end of the seminar, your group must create a short mini report or 3 to 5 slide presentation.

Your final work must include:

1. Website selected
2. Main user and user goal
3. Technical observation from Wireshark or DevTools
4. Performance issue from Lighthouse or DevTools
5. Accessibility issue from WAVE, axe or Lighthouse
6. UX/HCI issue found by the group
7. Redesign sketch or wireframe
8. Questionnaire or usability test plan
9. Final recommendation

---

# 2-Hour Seminar Task Plan

## Part 1: Website Selection and First Impression

### Time: 10 minutes

Choose your website and answer the following questions:

1. What website did you choose?
2. Who is the main user?
3. What is the main user goal?
4. What is the most important task on the website?
5. What is your first impression of the design?
6. What looks clear?
7. What looks confusing?

### Example

Website: Restaurant website  
Main user: Customer who wants to order food  
Main goal: View menu and contact/order from the restaurant  
Possible issue: Contact details are not easy to find  

### Deliverable

Write a short website profile:

```text
Website name:
Website type:
Main user:
Main user goal:
Main task:
First impression:
```

---

## Part 2: Technical Observation with Wireshark or Chrome DevTools

### Time: 20 minutes

Use Wireshark or Chrome DevTools to observe what happens when the website loads.

### Option A: Wireshark

Basic steps:

1. Open Wireshark.
2. Select your active network interface.
3. Start capture.
4. Open the selected website in your browser.
5. Wait until the page loads.
6. Stop capture.
7. Use filters to explore the traffic.

Useful filters:

```text
dns
tcp
tls
http
ip.addr == <server-ip>
```

Look for:

- DNS traffic
- TCP connections
- TLS/HTTPS traffic
- server IP addresses
- whether content is encrypted
- number of packets captured
- any unexpected domains or third-party requests

### Option B: Chrome DevTools

Basic steps:

1. Open the website.
2. Right-click and choose Inspect.
3. Open the Network tab.
4. Refresh the page.
5. Observe the files loaded.

Look for:

- number of requests
- page size
- loading time
- images loaded
- JavaScript files
- third-party domains
- failed requests

### Discussion Questions

1. What happens technically when the page loads?
2. Is the website using HTTPS?
3. Is the actual content readable in Wireshark, or encrypted?
4. How many requests or packets are involved?
5. What does this tell us about performance, privacy or security?

### Deliverable

Write 3 technical observations.

Example:

```text
Observation 1: The website used DNS to resolve the domain name.
Observation 2: The website used TLS/HTTPS, so page content was encrypted.
Observation 3: The browser loaded many images and scripts, which may affect performance.
```

---

## Part 3: Use NotebookLM to Organise Findings

### Time: 15 minutes

Use NotebookLM as a research and note organisation tool.

You can paste your observations, upload your notes, or write a short summary and ask NotebookLM to help structure it.

### Suggested NotebookLM Prompts

```text
Summarise our website investigation findings in simple language.
```

```text
Create a checklist for reviewing this website from an HCI perspective.
```

```text
Explain DNS, TCP, TLS and HTTPS in beginner-friendly language.
```

```text
Turn these notes into a short report structure.
```

```text
Create 8 user questionnaire questions based on our findings.
```

### Important Rule

Do not copy the output blindly.

You must check whether the output matches what your group actually observed.

### Deliverable

Create:

- one short AI-assisted summary
- one checklist
- one corrected explanation in your own words

Example:

```text
NotebookLM helped us organise our observations into technical, usability and accessibility findings. We corrected the summary by adding what we actually saw in Wireshark and Lighthouse.
```

---

## Part 4: Performance Audit with Lighthouse

### Time: 15 minutes

Use Chrome Lighthouse to audit the website.

### Steps

1. Open the website in Chrome.
2. Right-click and choose Inspect.
3. Open Lighthouse.
4. Run an audit.
5. Record the scores and key issues.

Check:

- Performance
- Accessibility
- Best Practices
- SEO

### Questions

1. What is the performance score?
2. What is the accessibility score?
3. What is the biggest performance issue?
4. Are there large images or unused scripts?
5. Does the website work well on mobile?

### Deliverable

Complete this table:

| Area | Finding | Why It Matters | Suggested Fix |
|---|---|---|---|
| Performance |  |  |  |
| Accessibility |  |  |  |
| Best Practices |  |  |  |
| Mobile Experience |  |  |  |

### Example

| Area | Finding | Why It Matters | Suggested Fix |
|---|---|---|---|
| Performance | Large images slow page loading | Users may leave if the page is slow | Compress images and use modern image formats |

---

## Part 5: Accessibility Audit with WAVE or axe

### Time: 15 minutes

Use WAVE Accessibility Checker, axe DevTools or Lighthouse Accessibility.

Check for:

- missing alt text
- low contrast
- missing form labels
- unclear buttons
- poor heading structure
- keyboard navigation issues
- empty links
- inaccessible icons

### Questions

1. Can all users read the text clearly?
2. Are images described properly?
3. Are buttons meaningful?
4. Can users navigate without a mouse?
5. Is colour being used as the only way to communicate meaning?

### Deliverable

Record at least 2 accessibility issues.

Example:

```text
Issue 1: Some images are missing alt text.
Why it matters: Screen reader users may not understand the image content.
Suggested fix: Add meaningful alt text to important images.
```

```text
Issue 2: Some text has low contrast.
Why it matters: Users with low vision may struggle to read it.
Suggested fix: Increase contrast between text and background.
```

---

## Part 6: UX and HCI Review

### Time: 15 minutes

Now review the website as an HCI designer.

Focus on:

- visual hierarchy
- grouping
- colour scheme
- regional structure
- navigation
- logo design
- time to complete
- ease of use
- accessibility
- user confidence

### Questions

1. What does the user notice first?
2. Is the main call-to-action clear?
3. Are related items grouped together?
4. Is the navigation easy to understand?
5. Is the logo clear and suitable?
6. Is the colour scheme effective?
7. Can users complete the main task quickly?
8. What may confuse users?
9. What would you improve first?

### HCI Principles to Consider

- Gestalt proximity
- Gestalt similarity
- common region
- visual hierarchy
- contrast
- consistency
- feedback
- accessibility
- simplicity
- cognitive load
- error prevention

### Deliverable

Identify 3 UX/HCI issues.

Example:

```text
Issue 1: The contact button is not visible enough.
HCI principle: Visual hierarchy.
Suggested fix: Make the contact button more prominent.
```

```text
Issue 2: Food items are not clearly grouped.
HCI principle: Proximity and common region.
Suggested fix: Use food cards with image, name, price and button grouped together.
```

```text
Issue 3: Button styles are inconsistent.
HCI principle: Similarity and consistency.
Suggested fix: Use one consistent button style for all primary actions.
```

---

## Part 7: Redesign One Section Using an Industry Tool

### Time: 25 minutes

Use one design tool to redesign one section of the website.

Recommended tools:

- Figma
- Stitch
- Uizard
- Canva
- Penpot
- FigJam
- Pen and paper

### Choose One Section to Redesign

- homepage hero section
- navigation menu
- restaurant menu section
- contact section
- login form
- product card
- booking form
- search/filter section
- footer

### Your Redesign Must Improve

- visual hierarchy
- grouping
- accessibility
- button clarity
- mobile-friendliness
- ease of use
- cognitive load

### Apply at Least 3 HCI Principles

Choose from:

- proximity
- similarity
- common region
- continuation
- contrast
- consistency
- feedback
- affordance
- accessibility
- error prevention
- simplicity

### If Using Stitch or AI Tool

You may use this prompt:

```text
Redesign a clean, accessible and mobile-friendly website section for [website type]. The target user is [user type]. The main goal is [user goal]. The design should have clear visual hierarchy, grouped information, consistent buttons, strong contrast, accessible text, and a clear call-to-action.
```

After generating the design, you must critique it using HCI principles.

Do not stop at the AI output.

### Deliverable

Create one redesigned section and annotate it.

Your annotation should include:

```text
Original issue:
Redesign decision:
HCI principle applied:
Expected user benefit:
Tool used:
```

### Example

```text
Original issue: Food menu items were difficult to scan.
Redesign decision: We created food cards with image, dish name, price, description and Order button.
HCI principle applied: Common region and proximity.
Expected user benefit: Users can understand each item more quickly and place orders with less effort.
Tool used: Figma.
```

---

## Part 8: Create a User Feedback Questionnaire

### Time: 10 minutes

Create a short questionnaire to test your redesign.

Use a 1 to 5 scale.

1 = Strongly disagree  
2 = Disagree  
3 = Neutral  
4 = Agree  
5 = Strongly agree  

### Required Variables

Your questionnaire should test at least 5 of the following:

- grouping
- colour scheme
- regional structure
- logo design
- time to complete
- ease of use
- efficiency
- accessibility
- satisfaction
- navigation clarity
- visual hierarchy

### Example Questions

1. The layout was easy to understand.
2. Related information was clearly grouped.
3. The colour scheme improved the overall experience.
4. The page structure helped me find information quickly.
5. The logo was simple and recognisable.
6. The main button was easy to find.
7. I completed the task quickly.
8. The design was easy to use.
9. The design felt accessible.
10. Overall, I was satisfied with the interface.

### Add One Open-Ended Question

```text
What is one thing you would improve in this design?
```

### Add One Task-Based Metric

Ask a user to complete one task.

Examples:

```text
Find the contact number.
Find the menu.
Find the order button.
Find opening hours.
Add one item to the basket.
Find course information.
```

Record:

```text
Task completed: Yes/No
Time taken:
Confusion observed:
User comment:
```

### Deliverable

Create at least:

- 8 rating questions
- 1 open-ended question
- 1 task-based metric

---

## Part 9: Final Group Presentation

### Time: 15 minutes

Each group presents for 2 to 3 minutes.

Use this structure:

```text
We selected this website:
The main user is:
The main user goal is:
From Wireshark/DevTools, we observed:
From Lighthouse, we found:
From WAVE/axe, we found:
The main HCI issue is:
We redesigned:
The HCI principles we applied are:
Our questionnaire will test:
Our final recommendation is:
```

---

# Final Submission Checklist

Your final group output should include:

- [ ] Website name
- [ ] Main user
- [ ] Main user goal
- [ ] Main task
- [ ] Wireshark or DevTools observation
- [ ] Lighthouse performance/accessibility finding
- [ ] WAVE/axe accessibility finding
- [ ] 3 UX/HCI issues
- [ ] Redesign sketch or screen
- [ ] HCI principle annotations
- [ ] Questionnaire with at least 8 questions
- [ ] Task-based usability metric
- [ ] Final recommendation

---

# Example Final Output

## Website Selected

Restaurant website

## Main User

Customer who wants to view menu and order food.

## Main User Goal

Find food options, check prices and contact/order from the restaurant.

## Technical Observation

The website used HTTPS/TLS traffic, meaning the content was encrypted.

## Performance Issue

Large images may slow down page loading.

## Accessibility Issue

Some images did not have alt text.

## HCI Issue

Food items were not clearly grouped, making the menu harder to scan.

## Redesign Idea

Use food cards with image, dish name, price, description and Order button.

## HCI Principles Applied

- proximity
- common region
- similarity
- accessibility
- visual hierarchy

## Questionnaire Variable

Grouping and ease of use.

## Final Recommendation

Improve the menu layout using clear food cards, stronger contrast and a visible order button.

---

# Reflection Questions

At the end of the task, answer individually:

1. Which tool was most useful and why?
2. What did the technical tools reveal?
3. What did the accessibility tools reveal?
4. What did the design review reveal?
5. How did your redesign improve the user experience?
6. What would you test next with real users?

---

# Key Learning Message

Modern HCI work is evidence-based.

Wireshark and DevTools help us understand what the system is doing.

Lighthouse and WAVE help us identify performance and accessibility issues.

NotebookLM helps us organise findings and create structured notes.

Figma, Stitch or Uizard help us redesign the interface.

Questionnaires help us collect user feedback.

Good HCI connects all of these together so design decisions are based on evidence, not guesswork.

---

# Closing Line

Wireshark shows what the system is doing.  
Accessibility tools show who may be excluded.  
Figma shows what can be improved.  
NotebookLM helps organise what was learned.  
HCI connects everything into a better user experience.
