# CSE134B-SS20-HW1
# Name: David De Santiago
# PID: A17001592

## Part 1. Homework Tasks and Answers

### Question 1. Introduction to Web Technologies

Deployed Netlify Site URL: [https://aquamarine-kleicha-f98b3b.netlify.app](https://aquamarine-kleicha-f98b3b.netlify.app)

Screenshot of the homepage with my name and major included:
![Deployed Homepage Screenshot](screenshots/homepagescreenshot.png)

### Question 2. Chrome DevTools - Network

#### Number of Requests by Content Type:
- **HTML:** 1
- **CSS:** 1
- **JavaScript:** 1
- **Font:** 1
- **Images:** 4 (PNG, GIF, JPEG)
- **Media:** 1
- **SVG:** 5
- **Favicon:** 1

#### Total Number of Requests:
16

#### Total Bytes Sent:
6.7 MB transferred, 6.9 MB resources

#### Waterfall Graph:
![Waterfall Graph Screenshot](screenshots/Waterfallgraphscreenshot.png)

### Question 3. Client-Side Inherently Insecure Demo

Screenshot of the changes made:
![Client-Side Insecure Demo Screenshot](screenshots/question3screenshot.png)

## Part 2. Screen Reader Navigation Experience

### Navigating ESPN.com:
- **Easy Parts:**
  - I was able to find the "Top Headlines" section relatively quickly because I am already familiar with the ESPN website layout. As someone passionate about sports, I frequently visit ESPN, so I had an idea of where to look for the headlines, even without visually navigating.
- **Difficult Parts:**
  - Navigating solely with the screen reader was challenging because I am not used to this method of interaction. Moving between headings and links using the commands felt unintuitive at times, especially when trying to locate specific sections.

### Navigating WebAIM.org:
- **Easy Parts:**
  - None. Navigating WebAIM.org using the screen reader was unfamiliar and confusing.
- **Difficult Parts:**
  - I was unable to locate the "Web Accessibility Virtual Training" page or the FAQ section to determine if the training is archived. The process felt difficult because I had no prior familiarity with the website and the structure wasn’t as clear or easy to follow using the screen reader.

### General Reflection:
- **Experience:**
  - Completing this task was both easy and hard at the same time. While the commands for skipping between headings and links were useful, I found the overall process challenging because I’m not accustomed to using a screen reader. This was a completely new experience for me, and it required a lot of focus and patience to understand how the navigation worked.

## Part 3. HTTP Response Headers + Network Analysis

### Question 1. HTTP Response Headers + Network Analysis

#### HTTP Response Headers
- **UCI Response Headers Screenshot (Part 1):**
  ![UCI Response Headers Part 1](screenshots/uciheaderscreenshotpt1.png)
- **UCI Response Headers Screenshot (Part 2):**
  ![UCI Response Headers Part 2](screenshots/uciheaderscreenshotpt2.png)

- **UCSD Response Headers Screenshot (Part 1):**
  ![UCSD Response Headers Part 1](screenshots/ucsdheaderscreenshotpt1.png)
- **UCSD Response Headers Screenshot (Part 2):**
  ![UCSD Response Headers Part 2](screenshots/ucsdheaderscreenshotpt2.png)

#### Analysis of HTTP Response Headers
- **UCI**:
  - **Positive Observations**:
    - `Strict-Transport-Security` enforces HTTPS.
    - `X-Frame-Options` and `X-XSS-Protection` are present, mitigating clickjacking and XSS attacks.
  - **Potential Issues**:
    - Missing `Content-Security-Policy` for enhanced security against XSS and other attacks.
  - **Data Breakdown**:
    - **Documents (HTML):** 1.04%
    - **Stylesheets (CSS):** 3.6%
    - **Scripts (JavaScript):** 14%
    - **Fonts:** 0.85%
    - **Images:** 78.1%

- **UCSD**:
  - **Positive Observations**:
    - `Cache-Control` ensures sensitive content isn’t cached locally.
    - `Content-Type` is properly set to `text/html; charset=UTF-8`.
  - **Potential Issues**:
    - Missing key security headers: `Strict-Transport-Security`, `X-Frame-Options`, and `X-XSS-Protection`.
  - **Data Breakdown**:
    - **Documents (HTML):** 0.93%
    - **Stylesheets (CSS):** 4.84%
    - **Scripts (JavaScript):** 14.5%
    - **Fonts:** 0.72%
    - **Images:** 79.03%

### Question 2. JavaScript Off

#### **UCSD:**
- **Visual Changes:**
  - The layout of the homepage remained mostly intact.
  - Some interactive elements like animations and pop-ups were missing.
  - Static content and navigation links were visible, but functionality was limited.
  - **Screenshot:**  
    ![UCSD No JavaScript](screenshots/ucsdquestion3screenshot.png)

- **Broken Features:**
  - Search bar functionality did not work.
  - Some dynamic elements such as drop-down menus and hover effects were disabled.
  - Interactive elements like forms did not function properly.

#### **Scripps:**
- **Visual Changes:**
  - The homepage was completely blank with no visible content.
  - This indicates that the site relies heavily on JavaScript to load and display content.
  - **Screenshot:**  
    ![Scripps No JavaScript](screenshots/scrippsquestion3screenshot.png)

- **Broken Features:**
  - All content failed to load due to heavy reliance on JavaScript.
  - The site was essentially non-functional.

#### **UCLA:**
- **Visual Changes:**
  - The layout was partially intact, with static content visible.
  - Dynamic elements like sliders or interactive news tiles were not operational.
  - **Screenshot:**  
    ![UCLA No JavaScript](screenshots/uclaquestion3screenshot.png)

- **Broken Features:**
  - Search functionality and interactive menus were non-functional.
  - Some images and videos failed to load, affecting the visual presentation.
  - Dynamic navigation and pop-ups were entirely disabled.