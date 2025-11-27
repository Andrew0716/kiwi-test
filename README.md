# 🥝 Kiwi - Lighthouse for Everyone 💡

**A Website Diagnostic Tool Similar to Google Lighthouse (By Kiwi Team)**

<br>

## ✨ Kiwi Planning Purpose & Background

- **Problem Identification:** Google's AI Overviews, Featured Snippets, and Helpful Content Updates are causing a sharp decline in organic traffic for bloggers and small website owners. Many expert blogs are being outranked by Reddit and forum content.
- **Solution:** An intuitive tool is needed for **bloggers and small business owners**, even without expert developer knowledge, to easily diagnose and improve their website's quality.
- **Kiwi's Vision:** Built on the powerful diagnostic capabilities of Google Lighthouse, Kiwi provides **easy-to-understand reports and actionable improvement suggestions** for non-developers, helping to boost website performance, accessibility, and SEO scores.

<br>

## ✨ Development Motivation

- **Lowering the Barrier to Entry:** While Lighthouse reports are accurate, terms like `CLI` and `Node.js` present a high entry barrier for end-users unfamiliar with technical environments.
- **Overcoming the Traffic Crisis:** Adapting to Google's algorithm changes makes continuously monitoring and improving a website's technical health essential, not optional.
- **Simplicity and Efficiency:** Without complex setup, users can simply enter a URL to receive a comprehensive diagnostic report for both **mobile and desktop environments**, complete with **easy-to-understand improvement points**.

<br>

## ✨ Kiwi's Core Features

1.  **Comprehensive Website Diagnostic Report:** Provides scores and detailed analysis across five key categories: Performance, Accessibility, Best Practices, SEO, and PWA.
2.  **Non-Developer Friendly Reports:** Instead of "Reduce unused JavaScript," it offers explanations like **"Unused JavaScript files are slowing down your page load. Consider removing or combining these scripts."**
3.  **Desktop & Mobile Analysis:** Offers different results based on the user-selected device type, accurately reflecting real-user environments.
4.  **Improvement Guides:** Provides practical guides and resource links for identified issues, explaining **'Why is this important?'** and **'How can I fix it?'**

<br>

## ✨ Kiwi Architecture Overview (Lighthouse-Based)

<img width="613" height="403" alt="image" src="https://github.com/user-attachments/assets/e0ffcbdf-0c92-47fe-94f5-7a52b0c572b8" />

Kiwi builds a user-friendly interface layer on top of the powerful open-source Google Lighthouse engine.

| Component | Description |
| :--------- | :-------- |
| **Runner** | The 'brain' of the Kiwi diagnostic process. It controls the overall workflow. |
| **Driver** | The 'hands and feet' that directly control the Chrome browser. It loads pages and collects data. |
| **Gatherers** | The 'data collectors' that gather real data like performance logs, network requests, and DOM information. |
| **Artifacts** | The 'bundle' of all raw data collected by the Gatherers. |
| **Audits** | The 'inspectors' that evaluate the Artifacts. They check each item and assign scores. |
| **Scoring** | The 'grading system' that combines audit results to calculate the final weighted scores. |
| **Report** | The final output (HTML) presented to the user – the 'Kiwi Report'. |

<br>

## ✨ Project Timeline

| Period | Phase | Specific Activities |
| :--------- | :-------- | :------- |
| Day 1 | Planning & Design | Market analysis (Google policy changes), Kiwi concept planning, tech stack selection |
| Day 2 | Frontend Development | User Interface (UI) & User Experience (UX) design, Dashboard and Report View development |
| Day 3 | Backend Development | Lighthouse Runner integration, user request queue management, report generation & storage API development |
| Day 4 | Integration & Improvement | Frontend-Backend connection, formatting reports for non-developers, performance optimization, deployment |

<br>

## ✨ Future Development (Revenue Models)

- **Free Version:** Basic website diagnosis and improvement suggestions.
- **Paid Subscription (SaaS):** Monthly/Annual fee (€5-€15). Provides **advanced metrics**, **improvement history tracking**, **priority support**, and **automated periodic diagnostics**.
- **Partnerships:** API integration with web hosting companies and CMS platforms.

<br>

## ✨ Lessons Learned from the Project

This project was a process of deeply understanding the internal structure of a complex open-source tool like Lighthouse (`Runner`, `Driver`, `Gatherers`, `Audits`, etc.) and contemplating how to present it most intuitively to the general user. Finding the right balance between technical sophistication and user convenience was the biggest challenge and achievement. Furthermore, analyzing the impact of Google's macro-level policy changes on countless content creators and attempting to solve that problem with technology was a highly meaningful endeavor. This project reaffirmed the critical importance of architectural design and user-centric development thinking.
