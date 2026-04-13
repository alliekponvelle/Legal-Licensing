<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Legal and Licensing</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700&family=Manrope:wght@400;500;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --panel: rgba(248, 239, 221, 0.96);
      --panel-soft: rgba(255, 248, 234, 0.86);
      --text: #2e1a40;
      --muted: #66507b;
      --purple: #71419b;
      --purple-deep: #29123f;
      --gold: #d7b15c;
      --gold-deep: #9b7427;
      --red: #b43b4d;
      --green: #368856;
      --line: rgba(113, 65, 155, 0.15);
      --shadow: 0 24px 60px rgba(8, 2, 15, 0.35);
      --radius: 28px;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      font-family: "Manrope", sans-serif;
      background:
        radial-gradient(circle at top left, rgba(215, 177, 92, 0.12), transparent 22%),
        radial-gradient(circle at 85% 15%, rgba(113, 65, 155, 0.24), transparent 24%),
        linear-gradient(160deg, #0f0618 0%, #1c0c2c 38%, #30124b 72%, #12081d 100%);
      color: #f9f0dc;
      line-height: 1.6;
      min-height: 100vh;
    }

    .page {
      width: min(1180px, calc(100% - 32px));
      margin: 0 auto;
      padding: 28px 0 56px;
    }

    .hero {
      position: relative;
      overflow: hidden;
      padding: 56px 42px;
      border-radius: 0 0 34px 34px;
      background: linear-gradient(140deg, #160920 0%, #341552 34%, #71419b 70%, #d7b15c 100%);
      box-shadow: var(--shadow);
      isolation: isolate;
    }

    .hero::before,
    .hero::after {
      content: "";
      position: absolute;
      border-radius: 50%;
      background: rgba(255,255,255,0.08);
      filter: blur(2px);
      z-index: -1;
    }

    .hero::before {
      width: 260px;
      height: 260px;
      top: -100px;
      right: -60px;
    }

    .hero::after {
      width: 180px;
      height: 180px;
      bottom: -60px;
      left: 10px;
    }

    .eyebrow,
    .section-label,
    .pill {
      display: inline-flex;
      align-items: center;
      padding: 7px 14px;
      border-radius: 999px;
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .eyebrow {
      background: rgba(255,255,255,0.14);
      border: 1px solid rgba(255,255,255,0.22);
      color: #fff5dd;
    }

    .section-label {
      background: rgba(215, 177, 92, 0.16);
      color: var(--purple);
      margin-bottom: 14px;
    }

    .pill {
      background: rgba(113, 65, 155, 0.1);
      color: var(--purple-deep);
      margin: 0 6px 8px 0;
      letter-spacing: 0.08em;
    }

    h1, h2, h3 {
      margin: 0;
      font-family: "Cinzel", serif;
      font-weight: 700;
      letter-spacing: 0.02em;
    }

    h1 {
      margin-top: 18px;
      font-size: clamp(2.6rem, 7vw, 5rem);
      line-height: 0.96;
      max-width: 11ch;
    }

    .hero p {
      max-width: 68ch;
      margin: 18px 0 0;
      font-size: 1.04rem;
      color: rgba(255, 248, 235, 0.92);
    }

    .hero-grid,
    .grid-2,
    .grid-3 {
      display: grid;
      gap: 16px;
      margin-top: 18px;
    }

    .hero-grid {
      grid-template-columns: repeat(4, minmax(0, 1fr));
      margin-top: 28px;
    }

    .grid-2 { grid-template-columns: repeat(2, minmax(0, 1fr)); }
    .grid-3 { grid-template-columns: repeat(3, minmax(0, 1fr)); }

    .hero-stat {
      padding: 16px;
      border-radius: 18px;
      background: rgba(255,255,255,0.12);
      border: 1px solid rgba(255,255,255,0.16);
      backdrop-filter: blur(8px);
    }

    .hero-stat strong {
      display: block;
      font-size: 1.2rem;
      margin-bottom: 4px;
      color: #fff5dd;
    }

    .section,
    .cta {
      margin-top: 18px;
      padding: 28px;
      background: var(--panel);
      color: var(--text);
      box-shadow: var(--shadow);
      border-radius: var(--radius);
      border: 1px solid rgba(255,255,255,0.28);
    }

    .section h2 {
      font-size: clamp(1.8rem, 4vw, 2.7rem);
      line-height: 1.02;
      margin-bottom: 12px;
    }

    .section p {
      margin: 0 0 14px;
      color: var(--muted);
    }

    .card,
    .lesson-card,
    .template-card,
    .warning-card {
      background: var(--panel-soft);
      border: 1px solid var(--line);
      border-radius: 22px;
      padding: 18px;
    }

    .lesson-card {
      border-top: 4px solid var(--purple);
    }

    .warning-card {
      border-top: 4px solid var(--red);
    }

    .template-card {
      border-top: 4px solid var(--green);
    }

    .card h3,
    .lesson-card h3,
    .template-card h3,
    .warning-card h3 {
      font-size: 1.08rem;
      color: var(--purple-deep);
      margin-bottom: 8px;
    }

    ul,
    ol {
      margin: 0;
      padding-left: 20px;
      color: var(--muted);
    }

    li { margin-bottom: 8px; }

    code,
    pre {
      font-family: Consolas, "Courier New", monospace;
    }

    pre {
      white-space: pre-wrap;
      margin: 12px 0 0;
      padding: 14px;
      border-radius: 16px;
      background: rgba(41, 18, 63, 0.08);
      border: 1px solid rgba(113, 65, 155, 0.12);
      color: var(--purple-deep);
      font-weight: 700;
    }

    a {
      color: var(--purple-deep);
      font-weight: 800;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 18px;
      overflow: hidden;
      border-radius: 18px;
      background: rgba(255, 248, 234, 0.72);
    }

    th,
    td {
      padding: 13px 14px;
      text-align: left;
      border-bottom: 1px solid var(--line);
      vertical-align: top;
      color: var(--muted);
      font-size: 0.95rem;
    }

    th {
      color: var(--purple-deep);
      background: rgba(215, 177, 92, 0.18);
      font-weight: 800;
    }

    tr:last-child td { border-bottom: 0; }

    .quote {
      padding: 18px;
      margin-top: 18px;
      border-radius: 22px;
      background: linear-gradient(135deg, rgba(215, 177, 92, 0.18), rgba(113, 65, 155, 0.08));
      border: 1px solid rgba(215, 177, 92, 0.22);
      color: var(--purple-deep);
      font-weight: 700;
    }

    .cta {
      text-align: center;
      background: linear-gradient(135deg, rgba(41, 18, 63, 0.98), rgba(113, 65, 155, 0.92));
      color: #fff4de;
    }

    .cta h2 {
      font-size: clamp(1.9rem, 4vw, 3rem);
      margin-bottom: 12px;
    }

    .cta p {
      max-width: 66ch;
      margin: 0 auto;
      color: rgba(255, 243, 221, 0.88);
    }

    @media (max-width: 980px) {
      .hero-grid,
      .grid-2,
      .grid-3 {
        grid-template-columns: 1fr;
      }

      table,
      thead,
      tbody,
      th,
      td,
      tr {
        display: block;
      }

      th { display: none; }

      td {
        border-bottom: 0;
        padding: 10px 14px;
      }

      tr {
        border-bottom: 1px solid var(--line);
        padding: 8px 0;
      }
    }

    @media (max-width: 640px) {
      .page {
        width: min(100% - 16px, 1180px);
      }

      .hero,
      .section,
      .cta {
        padding: 22px;
      }
    }
  </style>
</head>
<body>
  <div class="page">
    <section class="hero">
      <span class="eyebrow">Module 1</span>
      <h1>Legal and Licensing</h1>
      <p>Learn how to sell digital products, promote affiliate offers, use reviews, talk about results, and work with MRR or PLR products without misleading your audience or putting your business at risk.</p>
      <div class="hero-grid">
        <div class="hero-stat">
          <strong>Protect</strong>
          <span>Understand basic FTC rules for creators and sellers</span>
        </div>
        <div class="hero-stat">
          <strong>Disclose</strong>
          <span>Use clear affiliate, sponsorship, and product disclosures</span>
        </div>
        <div class="hero-stat">
          <strong>License</strong>
          <span>Know the difference between MRR, PLR, private use, and affiliate offers</span>
        </div>
        <div class="hero-stat">
          <strong>Sell Right</strong>
          <span>Use honest claims, real reviews, and safer sales language</span>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Important</div>
      <h2>Start With This Disclaimer</h2>
      <p>This module is for education and business awareness. It is not legal advice. If you need legal advice for your exact business, product, contract, refund policy, or licensing agreement, speak with a qualified attorney.</p>
      <div class="quote">The goal is simple: sell with clarity, protect your reputation, and help customers understand what they are buying.</div>
    </section>

    <section class="section">
      <div class="section-label">Module Promise</div>
      <h2>What Students Will Learn</h2>
      <div class="grid-3">
        <div class="card">
          <h3>FTC Basics</h3>
          <p>Students learn why social posts, emails, landing pages, live selling, testimonials, and affiliate links can count as advertising.</p>
        </div>
        <div class="card">
          <h3>Disclosures</h3>
          <p>Students learn when to disclose, where to put disclosures, and how to write them in plain language.</p>
        </div>
        <div class="card">
          <h3>Reviews and Testimonials</h3>
          <p>Students learn how to use proof responsibly without fake reviews, AI-generated testimonials, or misleading screenshots.</p>
        </div>
        <div class="card">
          <h3>Income Claims</h3>
          <p>Students learn how to talk about results without making guarantees or implying everyone will earn the same amount.</p>
        </div>
        <div class="card">
          <h3>MRR and PLR Licensing</h3>
          <p>Students learn how resale rights work and why they must read license terms before selling, editing, or rebranding a product.</p>
        </div>
        <div class="card">
          <h3>Safer Selling</h3>
          <p>Students leave with checklists, templates, and examples they can use before posting or launching an offer.</p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Lesson Plan</div>
      <h2>Full Module Outline</h2>
      <div class="grid-2">
        <div class="lesson-card">
          <span class="pill">Lesson 1</span>
          <h3>Why Legal and Licensing Basics Matter</h3>
          <p>Online creators are also marketers. If a student recommends a product, sells a digital download, promotes an affiliate link, or posts a customer result, they need to be honest and clear.</p>
          <ul>
            <li>Marketing should be truthful and not misleading.</li>
            <li>Customers should understand what they are buying.</li>
            <li>Relationships that affect trust should be disclosed.</li>
            <li>Fake reviews, fake screenshots, and fake income proof can create risk.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 2</span>
          <h3>Affiliate Links, Paid Posts, and Sponsored Content</h3>
          <p>If a creator earns money, receives free products, gets a discount, or has a business relationship with a brand, the audience should know.</p>
          <ul>
            <li>Affiliate commission should be disclosed.</li>
            <li>Free or discounted products should be disclosed.</li>
            <li>Paid partnerships should be disclosed clearly.</li>
            <li>Short, vague tags like #sp or #collab may not be clear enough for beginners.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 3</span>
          <h3>Where Disclosures Should Go</h3>
          <p>A disclosure should be easy to see before someone buys, clicks, or acts on the recommendation.</p>
          <ul>
            <li>Put disclosures near the claim, link, or call to action.</li>
            <li>Do not hide disclosures at the bottom of a long caption.</li>
            <li>Do not rely only on a profile bio.</li>
            <li>For videos, place disclosures on screen and say them out loud when possible.</li>
            <li>For emails and landing pages, place disclosures before the offer link or checkout button.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 4</span>
          <h3>Reviews, Testimonials, and Screenshots</h3>
          <p>Proof is powerful, but it needs to be real. Students should only use testimonials from real people with real experience.</p>
          <ul>
            <li>Do not create fake reviews or AI-generated testimonials.</li>
            <li>Do not use reviews from people who never used the product.</li>
            <li>Do not edit screenshots to exaggerate results.</li>
            <li>Ask permission before using customer screenshots.</li>
            <li>Disclose if a review was incentivized, paid, or connected to a free product.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 5</span>
          <h3>Income Claims and Results Claims</h3>
          <p>Students should avoid making it sound like income is guaranteed or typical for everyone.</p>
          <ul>
            <li>Do not promise guaranteed sales, followers, income, or business results.</li>
            <li>Do not imply every student will get the same result.</li>
            <li>Explain that results depend on niche, offer, audience, effort, consistency, pricing, and market demand.</li>
            <li>Use education-focused wording instead of guarantee-focused wording.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 6</span>
          <h3>MRR, PLR, Affiliate, and Private Use Licenses</h3>
          <p>Licensing tells students what they are allowed to do with a product. They should read the license before reselling, editing, rebranding, or giving anything away.</p>
          <ul>
            <li>MRR usually means master resale rights, but every license is different.</li>
            <li>PLR usually means private label rights, but editing rules vary.</li>
            <li>Affiliate offers pay commission but usually do not give ownership or resale rights.</li>
            <li>Private use products are for personal use and should not be resold unless the license says so.</li>
            <li>Students should keep a copy of every license they rely on.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 7</span>
          <h3>AI Content, Fake Proof, and Ethical Marketing</h3>
          <p>AI can help students write and organize, but it should not invent proof.</p>
          <ul>
            <li>AI can help draft emails, captions, FAQs, lesson summaries, and product descriptions.</li>
            <li>AI should not create fake customer reviews, fake case studies, fake income proof, or fake testimonials.</li>
            <li>Students should fact-check AI-generated marketing copy before publishing.</li>
            <li>Do not use AI to pretend a customer said something they never said.</li>
          </ul>
        </div>

        <div class="lesson-card">
          <span class="pill">Lesson 8</span>
          <h3>Before You Post or Sell Checklist</h3>
          <p>This lesson brings everything together into one simple review process students can use before launching an offer.</p>
          <ul>
            <li>Check the offer, claims, disclosures, testimonials, refund language, license terms, and checkout expectations.</li>
            <li>Make sure the customer understands what is included and what is not included.</li>
            <li>Use the templates in this module to make safer sales pages, captions, emails, and live scripts.</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Risky vs. Safer</div>
      <h2>Words Matter</h2>
      <table>
        <thead>
          <tr>
            <th>Risky Wording</th>
            <th>Safer Wording</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Make $10K/month with this system.</td>
            <td>This training shows the steps I use to build and promote digital offers. Results are not guaranteed.</td>
          </tr>
          <tr>
            <td>Guaranteed daily sales.</td>
            <td>This can help you create a clearer offer and a more consistent promotion plan.</td>
          </tr>
          <tr>
            <td>Anyone can make $500 today.</td>
            <td>Some students use this as a beginner-friendly income path, but results vary.</td>
          </tr>
          <tr>
            <td>Everyone loves this product.</td>
            <td>Here is real feedback from customers who gave permission to share their experience.</td>
          </tr>
          <tr>
            <td>No refunds ever, no matter what.</td>
            <td>Review the refund policy before purchasing so you understand how digital product access works.</td>
          </tr>
        </tbody>
      </table>
    </section>

    <section class="section">
      <div class="section-label">Templates</div>
      <h2>Copy and Paste Swipe File</h2>
      <div class="grid-2">
        <div class="template-card">
          <h3>Affiliate Disclosure</h3>
          <pre>Affiliate disclosure: I may earn a commission if you purchase through my link, at no extra cost to you.</pre>
        </div>
        <div class="template-card">
          <h3>Digital Product Seller Disclosure</h3>
          <pre>I created and sell this digital product, so I may earn from purchases.</pre>
        </div>
        <div class="template-card">
          <h3>Income Disclaimer</h3>
          <pre>Income Disclaimer: This training is for educational purposes only. Results are not guaranteed. Your results depend on your offer, niche, audience, effort, consistency, pricing, and market demand.</pre>
        </div>
        <div class="template-card">
          <h3>Testimonial Disclaimer</h3>
          <pre>Testimonials reflect individual experiences. Your results may vary.</pre>
        </div>
        <div class="template-card">
          <h3>Sponsored Content Disclosure</h3>
          <pre>Paid partnership with [Brand].</pre>
        </div>
        <div class="template-card">
          <h3>Free Product Disclosure</h3>
          <pre>[Brand] sent me this product for free, but these are my honest thoughts.</pre>
        </div>
        <div class="template-card">
          <h3>TikTok Shop Affiliate Disclosure</h3>
          <pre>TikTok Shop affiliate link: I may earn commission from qualifying purchases.</pre>
        </div>
        <div class="template-card">
          <h3>MRR / PLR License Reminder</h3>
          <pre>This product includes resale rights. Please review the license terms before reselling, editing, rebranding, or redistributing it.</pre>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Checklists</div>
      <h2>Student Downloads to Include</h2>
      <div class="grid-2">
        <div class="template-card">
          <h3>FTC-Safe Promo Checklist</h3>
          <ol>
            <li>Am I earning money from this link, product, or recommendation?</li>
            <li>Did I clearly disclose that relationship?</li>
            <li>Is the disclosure easy to notice before someone buys or clicks?</li>
            <li>Are my testimonials real?</li>
            <li>Did I get permission to use screenshots?</li>
            <li>Am I avoiding fake reviews or AI-generated proof?</li>
            <li>Am I avoiding guaranteed income or guaranteed results?</li>
            <li>Is my refund policy or digital product access policy clear?</li>
            <li>Would a beginner understand what they are buying?</li>
          </ol>
        </div>
        <div class="template-card">
          <h3>MRR / PLR License Review Checklist</h3>
          <ol>
            <li>Do I have the actual license terms saved?</li>
            <li>Am I allowed to resell the product?</li>
            <li>Am I allowed to edit or rebrand the product?</li>
            <li>Am I allowed to give customers resale rights?</li>
            <li>Am I allowed to sell it on my chosen platform?</li>
            <li>Are there minimum price rules?</li>
            <li>Are there claims I am not allowed to make?</li>
            <li>Do I know what customer support I am responsible for?</li>
          </ol>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Common Mistakes</div>
      <h2>What Students Should Avoid</h2>
      <div class="grid-3">
        <div class="warning-card">
          <h3>Hiding Disclosures</h3>
          <p>Do not bury affiliate or sponsorship disclosures at the bottom of a caption, only in a bio, or after a long wall of text.</p>
        </div>
        <div class="warning-card">
          <h3>Fake Proof</h3>
          <p>Do not use fake testimonials, fake customer screenshots, fake income dashboards, or AI-generated reviews.</p>
        </div>
        <div class="warning-card">
          <h3>Overpromising</h3>
          <p>Do not promise guaranteed income, viral growth, daily sales, or the same results for every student.</p>
        </div>
        <div class="warning-card">
          <h3>Ignoring Licenses</h3>
          <p>Do not resell, edit, or give away an MRR or PLR product unless the license clearly allows it.</p>
        </div>
        <div class="warning-card">
          <h3>Using Customer Screenshots Without Permission</h3>
          <p>Ask first. Save the permission. Blur private information before posting.</p>
        </div>
        <div class="warning-card">
          <h3>Confusing Affiliate With Ownership</h3>
          <p>An affiliate link does not mean the student owns the product or has the right to resell it.</p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Knowledge Check</div>
      <h2>Quick Student Quiz</h2>
      <div class="grid-2">
        <div class="card">
          <h3>Question 1</h3>
          <p>You earn commission from a link in your bio. Should you disclose it?</p>
          <div class="quote">Answer: Yes. Use clear language near the link or offer.</div>
        </div>
        <div class="card">
          <h3>Question 2</h3>
          <p>Can you use AI to invent customer reviews if the product is good?</p>
          <div class="quote">Answer: No. Reviews and testimonials should come from real customer experiences.</div>
        </div>
        <div class="card">
          <h3>Question 3</h3>
          <p>If a product says PLR, can you automatically sell it however you want?</p>
          <div class="quote">Answer: No. Read the actual license terms because every product can have different rules.</div>
        </div>
        <div class="card">
          <h3>Question 4</h3>
          <p>Is "guaranteed daily sales" a safe claim?</p>
          <div class="quote">Answer: No. It is safer to explain what the training teaches and state that results vary.</div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="section-label">Sources</div>
      <h2>Research Links</h2>
      <p>Use these as starting references when recording the lesson videos or creating student downloads.</p>
      <ul>
        <li><a href="https://www.ftc.gov/business-guidance/advertising-marketing">FTC Advertising and Marketing Basics</a></li>
        <li><a href="https://www.ftc.gov/business-guidance/resources/disclosures-101-social-media-influencers">FTC Disclosures 101 for Social Media Influencers</a></li>
        <li><a href="https://www.ftc.gov/business-guidance/resources/consumer-reviews-testimonials-rule-questions-answers">FTC Consumer Reviews and Testimonials Rule Q&A</a></li>
        <li><a href="https://www.ftc.gov/news-events/news/press-releases/2024/08/federal-trade-commission-announces-final-rule-banning-fake-reviews-testimonials">FTC Final Rule Banning Fake Reviews and Testimonials</a></li>
      </ul>
    </section>

    <section class="cta">
      <h2>Sell With Clarity</h2>
      <p>Legal and licensing basics are not meant to scare students. They are meant to help students sell smarter, protect their brand, and build trust with the people they serve.</p>
    </section>
  </div>
</body>
</html>
