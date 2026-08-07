# QHO542 Week 7 Technical HCI Activity

## Reverse Engineer a Live Website

### Goal

Choose any public website and technically inspect how it behaves from a UX point of view.

You are NOT redesigning the site yet.

Your job is to collect technical evidence about:

* page structure
* accessibility
* network behaviour
* performance
* responsive behaviour
* user interaction
* navigation
* loading behaviour

---

# Tools

Use:

* Chrome DevTools
* Lighthouse
* WAVE
* Microsoft Clarity only if you own/control the website
* Optional: PageSpeed Insights

---

# Important

If you are using a random public website such as:

* Amazon
* Airbnb
* Booking.com
* GOV.UK
* university website
* restaurant website

you can inspect it using DevTools, Lighthouse and WAVE.

You CANNOT add Microsoft Clarity tracking to a website you do not own.

Clarity requires access to the website code.

---

# TASK 1 — Choose a Live Website

Choose one website.

Example:

```text
https://www.gov.uk
```

or any other suitable live website.

Write down:

```text
Website:

Main purpose:

Main user:

Main task:
```

Example:

```text
Main task:
Find information about applying for a driving licence.
```

---

# TASK 2 — Inspect the HTML Structure

Open the website.

Right click:

```text
Inspect
```

Open:

```text
Elements
```

Look for:

```html
<header>
<nav>
main>
<section>
<button>
<a>
<form>
<input>
<img>
<footer>
```

Check:

```text
Is navigation inside <nav>?

Are buttons real <button> elements?

Are headings using h1, h2, h3 correctly?

Do images have alt attributes?

Are form fields labelled?
```

---

# HINT

You do not need to understand all the HTML.

Look only at the UI elements.

---

# TASK 3 — Keyboard Test

Do not use the mouse.

Use:

```text
TAB

SHIFT + TAB

ENTER

SPACE

ESC
```

Try to complete the main task.

Record:

```text
Can you see keyboard focus?

Does TAB move logically?

Can you access the menu?

Can you activate buttons?

Do you get stuck anywhere?

Can the task be completed?
```

---

# TASK 4 — Accessibility Inspection

Use:

```text
Chrome DevTools
→ Elements
→ Accessibility
```

Inspect:

```text
Buttons

Links

Forms

Images
```

Check:

```text
Accessible name

Role

ARIA label

Alt text

Keyboard focus
```

---

# Optional Tool

Open:

```text
https://wave.webaim.org/
```

Enter the website URL.

Look for:

```text
Errors

Contrast errors

Missing alt text

Heading problems

Form-label problems
```

Record at least 3 findings.

---

# TASK 5 — Run Lighthouse

Open:

```text
Chrome DevTools
→ Lighthouse
```

Select:

```text
Performance

Accessibility

Best Practices

SEO
```

Run the analysis.

Record:

```text
Performance score:

Accessibility score:

Best Practices score:

SEO score:
```

Then identify:

```text
1 performance issue

1 accessibility issue

1 best-practice issue
```

---

# TASK 6 — Network Inspection

Open:

```text
DevTools
→ Network
```

Reload the page.

Look at the requests.

Identify:

```text
HTML

CSS

JavaScript

Images

Fonts

Fetch/XHR
```

Record:

```text
Total number of requests:

Approximate transferred data:

Approximate page load time:
```

---

# HINT

Use the Network filters:

```text
Fetch/XHR

JS

CSS

Img

Font

Doc
```

This helps you understand what the browser downloads to build the interface.

---

# TASK 7 — Find the API Calls

Inside:

```text
Network
→ Fetch/XHR
```

Interact with the website.

Try:

```text
Search

Apply filter

Open product

Change category

Submit search
```

Watch whether new network requests appear.

Click one request.

Inspect:

```text
Headers

Payload

Response

Timing
```

---

# Challenge

Try to answer:

```text
What action triggered this request?

What endpoint was called?

What data was sent?

What data came back?
```

Do NOT modify or attack the request.

Observation only.

---

# TASK 8 — Performance Throttling

Open:

```text
Network
```

Find throttling.

Change from:

```text
No throttling
```

to a slower network profile if available.

Reload.

Observe:

```text
What appears first?

What appears late?

Are images delayed?

Can you interact while loading?

Does content move while loading?

Is there a loading indicator?
```

---

# Question

Would this experience still be usable on a slow mobile connection?

---

# TASK 9 — Responsive Reverse Engineering

Open:

```text
DevTools
→ Toggle Device Toolbar
```

Test:

```text
Mobile

Tablet

Desktop
```

Watch how the site changes.

Record:

```text
Navigation changes:

Layout changes:

Elements hidden:

Elements moved:

Text changes:

Button changes:
```

---

# Challenge

Find one element that changes significantly between mobile and desktop.

Example:

```text
Desktop:
Full navigation menu

Mobile:
Hamburger menu
```

Explain why that decision may have been made.

---

# TASK 10 — Check Page Performance More Deeply

Open:

```text
https://pagespeed.web.dev/
```

Paste the website URL.

Run the test.

Compare:

```text
Mobile

Desktop
```

Look at:

```text
Largest Contentful Paint

Interaction to Next Paint

Cumulative Layout Shift
```

You do not need to memorise the numbers.

Understand what they mean.

---

# Simple Meaning

```text
LCP
How quickly the main visible content loads.

INP
How quickly the website responds when the user interacts.

CLS
How much the interface unexpectedly moves around.
```

These are technical metrics that directly affect user experience.

---

# TASK 11 — Reverse Engineer the User Journey

Choose ONE task.

Example:

```text
Search for a hotel.
```

Complete it normally.

Record every step.

Example:

```text
Homepage

→ Search field

→ Enter location

→ Select dates

→ Search

→ Results

→ Apply filter

→ Select hotel
```

Count:

```text
Number of clicks:

Number of pages:

Number of decisions:

Number of form fields:

Number of scrolls:
```

---

# TASK 12 — Find Technical UX Problems

Based on all your testing, identify 5 problems.

Use this format:

```text
Problem:

Technical evidence:

User impact:
```

Example:

```text
Problem:
Large hero image loads slowly.

Technical evidence:
Image request is one of the largest resources in Network.

User impact:
Important content appears later on slow connections.
```

---

# TASK 13 — Final Technical Evidence Table

Complete:

| Area              | Evidence | UX Impact |
| ----------------- | -------- | --------- |
| HTML Structure    |          |           |
| Keyboard          |          |           |
| Accessibility     |          |           |
| Lighthouse        |          |           |
| Network           |          |           |
| API/XHR           |          |           |
| Performance       |          |           |
| Responsive Design |          |           |

---

# Final Challenge

You should be able to explain:

```text
How is the website structured?

How does the browser load it?

What happens when the user clicks something?

Does the website call an API?

How does it behave on slow internet?

How does it change on mobile?

Can it be used without a mouse?

What technical problems could affect UX?
```

---

# Final Output

Submit:

```text
Website URL

Screenshot of DevTools Elements

Screenshot of Network requests

Lighthouse scores

WAVE findings

One API/XHR observation

One mobile vs desktop observation

Five technical UX findings
```

---

# Important Rule

This activity is for:

```text
Observation

Analysis

HCI evaluation
```

Do NOT:

```text
Attack the website

Bypass authentication

Modify requests

Attempt exploitation

Access data you are not authorised to access
```

Stay within normal browser inspection and public behaviour.

---

# Key Message

A website is not only what you see on the screen.

Behind the interface you have:

```text
HTML
CSS
JavaScript
APIs
Network requests
Accessibility structure
Performance behaviour
Responsive logic
```

All of these affect the user experience.

