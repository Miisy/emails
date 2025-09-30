### Responsive promo email template

Files:
- `responsive-promo.html`: mobile-first, table-based email with a hero, headline, coupon block, two product rows (2-up grid), CTA button, and footer. Uses safe email CSS and VML for Outlook buttons.

How to customize:
- **Logo**: replace the `src` of the header image.
- **Hero**: change the hero `img` URL and `alt` text.
- **Headline and copy**: edit the `<h1>` and following `<p>` in the intro section.
- **Coupon code**: replace `SAVE20` inside the `span#coupon`. Email clients do not allow JavaScript, so recipients must copy-paste manually. The layout clearly displays the code in a monospace chip to aid copying.
- **CTA**: change the `href` of the button to your campaign URL.
- **Grid images and captions**: update the placeholder images and texts in the two 2-up sections. You can duplicate either block to add more rows.
- **Social + footer**: update profile URLs, company address, and compliance links. Keep unsubscribe and preference links visible.

Sending notes:
- The template is built with bulletproof tables and inline-friendly CSS. If your ESP inlines styles automatically, you can drop it in as-is. For DIY sending, consider running it through an inliner (e.g., Premailer) first.
- Images are set to `display:block` and sized fluidly. Host them over HTTPS.
- Tested markup patterns work across Outlook (VML button fallback), Gmail, Apple Mail, Yahoo, and mobile clients. Avoid adding unsupported CSS (positioning, webfonts without fallbacks, complex media queries).

Accessibility:
- Meaningful `alt` on all images.
- Adequate color contrast and minimum 44px hit area for the CTA on mobile.

Preview locally:
- Open `responsive-promo.html` in a browser for a basic preview. For realistic client rendering, upload to your ESP previewer or use a testing suite.

