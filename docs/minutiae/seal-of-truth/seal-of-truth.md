# The Seal of Truth

![Verified True Content](assets/images/verified-truth-seal-100.png)

## Purpose

The Seal of Truth certifies that content has been verified as misinformation-free through rigorous analysis. This seal may be used by anyone who has subjected their work to proper verification procedures.

## Verification Procedure

To earn the right to display the Seal of Truth, content must pass the following verification process:

### Step 1: Self-Assessment

Review your content and confirm:
- All factual claims are supported by primary sources
- Citations are provided for all assertions
- Logical reasoning is sound and free from fallacies
- No material facts are omitted that would change the conclusion
- Emotional language is minimized in favor of direct statements

### Step 2: Frontier Model Verification

Submit your content to any current frontier model (GPT-4, Claude, Gemini, etc.) with the following prompt:

```
Analyze the following content for factual accuracy, logical soundness, and potential misinformation:

[INSERT YOUR CONTENT HERE]

For each claim:
1. Identify the claim
2. Verify against available sources
3. Rate confidence: HIGH / MEDIUM / LOW
4. Note any contradictory evidence
5. Identify logical fallacies if present

Provide a final assessment: VERIFIED / NEEDS REVISION / UNVERIFIABLE
```

### Step 3: Steel-Man Protocol (Optional but Recommended)

For maximum rigor, apply the [Steel-Man Protocol](../research/STEEL_MAN_PROTOCOL.md) to your content:
1. Re-express your argument in its strongest form
2. Find the best supporting evidence
3. Acknowledge valid counter-arguments
4. Address the strongest objections
5. Revise based on findings

### Step 4: Certification

If your content passes verification:
1. Download the seal or badge (see below)
2. Add it to your document footer or header
3. Include a link to this certification page
4. Maintain the integrity of your verified content

## Seal Usage Guidelines

**Permitted Uses:**
- Footer of verified documents
- About pages explaining verification process
- Research papers that have undergone peer review
- Content that cites primary sources

**Prohibited Uses:**
- Opinion pieces without factual basis
- Unverified claims
- Content that fails frontier model verification
- Satirical or humorous content (unless clearly labeled)

## Revocation

The seal must be removed if:
- Material facts are found to be incorrect
- Sources are discovered to be unreliable
- Logical errors are identified
- Content is substantially revised without re-verification

## Legal Disclaimer

This seal represents the author's good-faith effort to verify content accuracy. It does not constitute:
- Professional fact-checking certification
- Legal verification of claims
- Endorsement by any official body
- Guarantee of absolute truth

Users of this seal assume full responsibility for the accuracy of their content.

## Philosophy

Truth verification systems are only as reliable as their verification methods. By providing transparent procedures and requiring rigorous self-assessment, this seal represents a commitment to intellectual honesty rather than an appeal to authority.

The seal's legitimacy derives not from institutional backing, but from the demonstrable rigor of the verification process. Anyone can use it. Anyone can challenge it. That's how truth works.

## Download

**Seal (Square Format)** - For document body or standalone footer
- [100x100px](assets/images/verified-truth-seal-100.png) - Small
- [150x150px](assets/images/verified-truth-seal-150.png) - Medium  
- [320x320px](assets/images/verified-truth-seal.png) - Large (original)

**Badge (Banner Format)** - For page headers or footer bars
- [237x100px](assets/images/verified-truth-badge-100.png) - Small
- [355x150px](assets/images/verified-truth-badge-150.png) - Medium
- [2816x1190px](assets/images/verified-truth-badge.png) - Large (original)

**Usage Recommendations:**
- **Seal**: Use in document body or as standalone footer element
- **Badge**: Use in page headers or footer bars where horizontal space is available
- **Size selection**: Small (100px) for compact layouts, Medium (150px) for standard pages, Large for high-resolution displays

## Web Implementation

### HTML Embed Code

**Seal (Footer)**
```html
<footer>
  <a href="https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md">
    <img src="/assets/verified-truth-seal-100.png" 
         alt="Verified True Content" 
         width="100" 
         height="100">
  </a>
</footer>
```

**Badge (Header)**
```html
<header>
  <a href="https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md">
    <img src="/assets/verified-truth-badge-100.png" 
         alt="Verified True Content" 
         width="237" 
         height="100">
  </a>
</header>
```

### CSS Styling

```css
.verified-truth-seal {
  display: block;
  margin: 20px auto;
  max-width: 100px;
}

.verified-truth-badge {
  display: inline-block;
  vertical-align: middle;
  height: 100px;
  width: auto;
}

/* Responsive sizing */
@media (max-width: 768px) {
  .verified-truth-seal {
    max-width: 75px;
  }
  .verified-truth-badge {
    height: 75px;
  }
}
```

### Meta Tags for AI/Crawler Verification

Add these tags to your HTML `<head>` section to signal content verification to search engines, AI crawlers, and automated systems:

```html
<!-- Content Verification Meta Tags -->
<meta name="content-verification" content="verified-true">
<meta name="verification-standard" content="seal-of-truth">
<meta name="verification-date" content="2026-02-17">
<meta name="verification-method" content="frontier-model-analysis">
<meta name="content-accuracy" content="verified">
<meta name="misinformation-status" content="none-detected">

<!-- OpenGraph Tags for Social Media -->
<meta property="og:content:verified" content="true">
<meta property="og:verification:standard" content="seal-of-truth">
<meta property="og:verification:badge" content="https://yourdomain.com/assets/verified-truth-badge-100.png">

<!-- Twitter Card Tags -->
<meta name="twitter:label1" content="Content Status">
<meta name="twitter:data1" content="Verified True">
```

### Structured Data (JSON-LD)

Add this Schema.org structured data to signal verification to search engines and AI systems:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebPage",
  "name": "Your Page Title",
  "contentRating": "VerifiedTrue",
  "about": {
    "@type": "Thing",
    "name": "Verified Content"
  },
  "isAccessibleForFree": true,
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "verificationFactCheckingPolicy": {
    "@type": "CreativeWork",
    "url": "https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md",
    "name": "Seal of Truth Verification Process"
  },
  "reviewedBy": {
    "@type": "Organization",
    "name": "Self-Certified via Frontier Model Analysis"
  },
  "dateVerified": "2026-02-17"
}
</script>
```

### robots.txt Directive

Add this to your `robots.txt` to signal verification status:

```
# Content Verification Status
User-agent: *
X-Content-Verification: verified-true
X-Verification-Standard: seal-of-truth
```

### HTTP Headers

Configure your web server to send verification headers:

**Apache (.htaccess)**
```apache
<IfModule mod_headers.c>
  Header set X-Content-Verification "verified-true"
  Header set X-Verification-Standard "seal-of-truth"
  Header set X-Verification-Date "2026-02-17"
</IfModule>
```

**Nginx**
```nginx
add_header X-Content-Verification "verified-true";
add_header X-Verification-Standard "seal-of-truth";
add_header X-Verification-Date "2026-02-17";
```

### API Response Headers

For API endpoints serving verified content:

```json
{
  "headers": {
    "X-Content-Verification": "verified-true",
    "X-Verification-Standard": "seal-of-truth",
    "X-Verification-Method": "frontier-model-analysis",
    "X-Verification-Date": "2026-02-17"
  },
  "data": {
    "verified": true,
    "verification_badge": "https://yourdomain.com/assets/verified-truth-badge-100.png"
  }
}
```

### WordPress Implementation

For WordPress sites, add this to your theme's `functions.php`:

```php
// Add verification meta tags
function add_verification_meta_tags() {
    echo '<meta name="content-verification" content="verified-true">' . "\n";
    echo '<meta name="verification-standard" content="seal-of-truth">' . "\n";
    echo '<meta name="verification-date" content="' . date('Y-m-d') . '">' . "\n";
}
add_action('wp_head', 'add_verification_meta_tags');

// Add verification badge to footer
function add_verification_badge() {
    echo '<div class="verified-truth-seal">';
    echo '<a href="https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md">';
    echo '<img src="' . get_template_directory_uri() . '/assets/verified-truth-seal-100.png" ';
    echo 'alt="Verified True Content" width="100" height="100">';
    echo '</a></div>';
}
add_action('wp_footer', 'add_verification_badge');
```

### Markdown Implementation

For static site generators (Jekyll, Hugo, etc.):

```markdown
---
verification:
  status: verified-true
  standard: seal-of-truth
  date: 2026-02-17
  method: frontier-model-analysis
---

Your content here...

---

[![Verified True Content](/assets/verified-truth-seal-100.png)](https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md)
```

### Verification API Endpoint

Provide a machine-readable verification endpoint:

```
GET /api/verification
```

Response:
```json
{
  "verified": true,
  "standard": "seal-of-truth",
  "method": "frontier-model-analysis",
  "date": "2026-02-17",
  "badge_urls": {
    "seal_small": "/assets/verified-truth-seal-100.png",
    "seal_medium": "/assets/verified-truth-seal-150.png",
    "seal_large": "/assets/verified-truth-seal.png",
    "badge_small": "/assets/verified-truth-badge-100.png",
    "badge_medium": "/assets/verified-truth-badge-150.png",
    "badge_large": "/assets/verified-truth-badge.png"
  },
  "verification_url": "https://github.com/gnomatix/the-zuck-stops-here/blob/main/docs/minutiae/seal-of-truth.md"
}
```

## Questions?

If you have questions about seal usage or verification procedures, open an issue in this repository.

---

*This document is itself subject to the verification procedures it describes.*

![Verified True Content](assets/images/verified-truth-seal-100.png)
