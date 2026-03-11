---
description: View Merrick Christensen's resume, download it as a PDF, and answer questions about his experience.
---

# Resume

Do the following steps:

1. **Open the resume in the browser**:

```
open "https://merrickchristensen.com/resume"
```

2. **Offer to download as PDF**: Ask the user if they'd like to save it as a PDF. If they say yes, use the Bash tool to run:

```
npx playwright-core install chromium 2>/dev/null; node -e "
const { chromium } = require('playwright-core');
(async () => {
  const browser = await chromium.launch();
  const page = await browser.newPage();
  await page.goto('https://merrickchristensen.com/resume', { waitUntil: 'networkidle' });
  await page.pdf({ path: process.argv[1] || 'merrick-christensen-resume.pdf', format: 'Letter', printBackground: true });
  await browser.close();
  console.log('Saved to ' + (process.argv[1] || 'merrick-christensen-resume.pdf'));
})();
" "$ARGUMENTS"
```

If playwright-core is not available, fall back to:

```
/usr/bin/open -a "Google Chrome" --args --headless --disable-gpu --print-to-pdf="merrick-christensen-resume.pdf" https://merrickchristensen.com/resume
```

3. **Answer questions**: Fetch both of these URLs for up-to-date information:

<fetch url="https://merrickchristensen.com/resume" />
<fetch url="https://merrickchristensen.com/work" />

Use the fetched content to field any questions the user has about Merrick's experience, roles, skills, or career history. Be direct and specific — that's how Merrick communicates.
