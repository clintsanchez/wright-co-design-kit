# Universal Client Social Media Template System

You are acting as a senior brand designer, design systems architect, social media designer, information designer, and art director.

Your task is to take the **existing design system for the CURRENT CLIENT** and extend it into a complete, reusable social media and digital content template library.

This is a universal system that will be used across many different client brands.

The current client's design system is always the source of truth.

Do not assume:

- A specific company name
- A specific logo
- A specific color palette
- A specific mascot
- A specific font
- A specific visual style
- A specific industry
- A specific brand personality

Everything must derive from the client design system that has already been created.

---

# 1. FIRST: READ THE ACTIVE CLIENT DESIGN SYSTEM

Before creating any templates, inspect the design system currently available in the project.

Extract and understand:

- Client name
- Brand positioning
- Logo system
- Logo variants
- Brand colors
- Semantic colors
- Typography
- Type scale
- Font weights
- Spacing system
- Grid system
- Border radius
- Borders
- Shadows
- Illustration style
- Photography style
- Iconography
- Graphic treatments
- Patterns
- Textures
- Gradients
- Background treatments
- Buttons
- Cards
- Badges
- Calls to action
- Brand personality
- Brand voice
- Visual hierarchy
- Accessibility rules
- Mascot or character system, if one exists
- Other brand specific components

Do not begin designing templates until you understand the design system.

---

# 2. DESIGN SYSTEM DEPENDENCY

Every social template must inherit from the active client design system.

The relationship should work like this:

CLIENT DESIGN SYSTEM

↓

SOCIAL CONTENT DESIGN SYSTEM

↓

CONTENT TEMPLATE FAMILY

↓

PLATFORM FORMAT

↓

FINAL ASSET

Do not hard code client specific styling into the social template architecture.

Instead, use semantic design tokens.

Examples:

`brand.primary`

`brand.secondary`

`brand.accent`

`surface.primary`

`surface.secondary`

`text.primary`

`text.secondary`

`border.default`

`radius.card`

`spacing.section`

`type.display`

`type.heading`

`type.body`

`type.caption`

`logo.primary`

`logo.inverse`

`image.style`

`icon.style`

The exact values come from the current client design system.

---

# 3. DO NOT REDESIGN THE CLIENT

Do not create a new visual identity.

Do not reinterpret the client's brand.

Do not invent:

- New colors
- New fonts
- New logo treatments
- New mascots
- New illustration styles
- New photography styles
- New gradients
- New icon systems

unless the existing design system explicitly allows them.

Extend the existing system.

Do not replace it.

---

# 4. BRAND ADAPTATION LOGIC

Different clients may have very different design systems.

The template architecture must support brands that are:

- Light
- Dark
- Minimal
- Bold
- Corporate
- Industrial
- Luxury
- Playful
- Technical
- Traditional
- Modern
- Service based
- Ecommerce
- B2B
- B2C
- Local business
- National brand
- Nonprofit
- Government
- Professional services

The layout architecture should remain reusable while the visual expression changes according to the active design system.

---

# 5. OPTIONAL BRAND ELEMENTS

Some clients may have:

- Mascots
- Characters
- Founders used heavily in branding
- Product photography
- Service photography
- Vehicles
- Equipment
- Branded uniforms
- Custom illustration systems
- Custom icon systems
- Patterns
- Textures
- Signature graphic devices

If present, create optional component slots for them.

Do not assume these elements exist.

For example:

`Brand Character / Hero`

should only exist when the design system contains a brand character.

Do not manufacture one.

---

# 6. PRIMARY OBJECTIVE

Create a complete reusable template system covering:

- Social media feed graphics
- Portrait social graphics
- Landscape social graphics
- Square graphics
- Stories
- Reels
- Short form video covers
- Social banners
- Social headers
- Avatars
- Profile images
- YouTube banners
- YouTube thumbnails
- Video covers
- Link previews
- Carousels
- Quote graphics
- Review graphics
- Testimonial graphics
- Statistics
- Charts
- Graphs
- Data visualization
- Infographics
- Comparison graphics
- Case studies
- Reports
- Audits
- Announcements
- Offers
- Promotions
- Educational graphics
- FAQs
- Checklists
- Timelines
- Processes
- Before and after graphics
- Problem and solution graphics
- Event graphics
- Hiring graphics
- Community graphics
- Blog promotion
- Podcast promotion
- Webinar promotion
- Client results
- Thought leadership
- Industry commentary
- Branded memes where appropriate

Create a SYSTEM rather than isolated examples.

---

# 7. RESPONSIVE MASTER FORMAT SYSTEM

Build reusable master layout families.

## Square

1080 × 1080

Ratio: 1:1

## Portrait Feed

1080 × 1350

Ratio: 4:5

## Full Screen Portrait

1080 × 1920

Ratio: 9:16

## Tall Content

1000 × 1500

Ratio: 2:3

## Social Landscape

1200 × 630

Ratio: approximately 1.91:1

## Standard Widescreen

1920 × 1080

Ratio: 16:9

## YouTube Thumbnail

1280 × 720

Ratio: 16:9

## Wide Banner

1500 × 500

Ratio: 3:1

## Ultra Wide Header

1584 × 396

Ratio: 4:1

Use these as reusable layout families.

Platform specific templates can inherit from them.

---

# 8. RESPONSIVE DESIGN RULE

Never take one composition and simply resize it.

Recompose designs intelligently.

For example:

A 4:5 statistic post may use:

- Statistic on left
- Supporting visual on right

Its 9:16 version may use:

- Statistic at top
- Visual in center
- Supporting copy below

Its landscape version may use:

- Visual left
- Statistic right

Same content.

Same brand.

Same hierarchy.

Different composition.

---

# 9. SOCIAL PLATFORM TEMPLATE LIBRARY

Create current platform specific templates.

Use platform appropriate dimensions and safe zones.

Platform specifications can change over time, so organize dimensions as editable configuration values rather than embedding them permanently into unrelated components.

---

# INSTAGRAM

Create:

- Feed Square: 1080 × 1080
- Feed Portrait: 1080 × 1350
- Feed Landscape: 1080 × 566
- Story: 1080 × 1920
- Reel Cover: 1080 × 1920
- Carousel Square
- Carousel Portrait
- Profile Image Master: 320 × 320

Include interface safe zones.

---

# FACEBOOK

Create:

- Feed Square: 1080 × 1080
- Feed Portrait: 1080 × 1350
- Feed Landscape
- Story: 1080 × 1920
- Reel Cover: 1080 × 1920
- Page Cover: 851 × 315
- Group Cover
- Event Cover
- Link Preview: 1200 × 630
- Profile Image

Include mobile and desktop cover crop zones.

---

# LINKEDIN

Create:

- Landscape Post: 1200 × 627
- Square Post: 1200 × 1200
- Portrait Post: 720 × 900
- Personal Profile Banner: 1584 × 396
- Company Cover: 1128 × 191
- Company Logo: 400 × 400
- Carousel Slide: 1080 × 1080
- Link Preview: 1200 × 627

---

# X

Create:

- Landscape: 1280 × 720
- Portrait: 720 × 1280
- Square: 1080 × 1080
- Header: 1500 × 500
- Profile Image: 400 × 400
- Link Preview

---

# THREADS

Create:

- Square
- Portrait
- Landscape
- Link Preview
- Profile Image

Use the appropriate shared master ratios.

---

# BLUESKY

Create:

- Square
- Portrait
- Landscape
- Profile Image
- Banner
- Link Preview

Account for responsive banner cropping.

---

# TIKTOK

Create:

- Vertical Post: 1080 × 1920
- Video Cover: 1080 × 1920
- Story: 1080 × 1920
- Landscape Ad: 1920 × 1080
- Square Ad
- Profile Image: 200 × 200

Include interface safe zones.

---

# YOUTUBE

Create:

- Video Thumbnail: 1280 × 720
- Channel Banner: 2560 × 1440
- Podcast Playlist Thumbnail: 1280 × 1280
- Profile Image: 800 × 800
- Community Square
- Community Portrait
- Community Landscape

For the channel banner, use the platform safe zone for critical text and logos.

YouTube currently recommends a 2560 × 1440 channel banner and a 1280 × 720 video thumbnail.

---

# PINTEREST

Create:

- Standard Pin: 1000 × 1500
- Square Pin: 1000 × 1000
- Landscape Cover: 800 × 450
- Profile Image: 280 × 280
- Educational Pin
- Checklist Pin
- Infographic Pin
- Blog Pin
- Data Pin

---

# SNAPCHAT

Create:

- Story: 1080 × 1920
- Ad: 1080 × 1920
- Profile Image
- Banner

Include interface safe zones.

---

# REDDIT

Create:

- Square
- Portrait
- Landscape
- Community Banner
- Community Icon
- AMA Graphic
- Discussion Graphic
- Data Graphic

---

# MASTODON

Create:

- Square
- Portrait
- Landscape
- Header
- Profile Image
- Link Preview

---

# GOOGLE BUSINESS PROFILE

Create:

- Update Graphic
- Square Graphic
- Landscape Graphic
- Offer
- Event
- Product
- Service
- Review
- Announcement
- Cover Style Image
- Logo Image

Prioritize readability at small display sizes.

---

# 10. UNIVERSAL AVATAR SYSTEM

Create an avatar system derived from the client's identity.

Possible variants:

- Primary logo
- Symbol
- Monogram
- Brand mark
- Character head
- Founder portrait

Only create variants supported by the client's brand system.

Use a high resolution master.

Include previews for:

- Square
- Circular crop
- 32 px
- 64 px
- 128 px
- 256 px

Keep primary information inside a central safe area.

---

# 11. CONTENT TEMPLATE FAMILIES

For applicable aspect ratios, create templates for:

## Statement

- Eyebrow
- Headline
- Supporting copy
- Optional CTA

## Statistic

- Large statistic
- Context
- Source
- Date
- Optional interpretation

## Quote

- Quote
- Attribution
- Company
- Optional photo

## Testimonial

- Rating
- Testimonial
- Name
- Optional location
- Optional company

## Review

Support:

- Google reviews
- Facebook reviews
- Client testimonials
- Platform independent reviews

## Problem

Single pain point.

## Problem And Solution

Split or sequential structure.

## Problem, Agitation, Solution

Three stage storytelling.

## Tips

Support:

- 3
- 5
- 7
- 10

## Checklist

Support:

- Short checklist
- Long checklist
- Audit checklist
- Process checklist

## Comparison

Support:

- A versus B
- Old versus new
- Good versus bad
- Before versus after
- Option comparison
- Feature comparison

## Myth Versus Fact

Support single graphics and carousel sequences.

## FAQ

Support:

- Single question
- FAQ card
- FAQ carousel
- FAQ cover

## Case Study

Support:

- Cover
- Challenge
- Strategy
- Solution
- Result
- Metrics
- Testimonial
- CTA

## Announcement

Support:

- Launch
- New service
- New employee
- Partnership
- Award
- Certification
- Event
- Milestone

---

# 12. CHART DESIGN SYSTEM

Build chart components that inherit from the current client's design tokens.

Create:

- Vertical bar
- Horizontal bar
- Grouped bar
- Stacked bar
- 100 percent stacked bar
- Line chart
- Multi series line chart
- Area chart
- Pie chart
- Donut chart
- Scatter chart
- Bubble chart
- Funnel
- Waterfall
- Gauge
- Progress bar
- Progress ring
- Sparkline
- Heat map
- Ranking chart
- Timeline
- Comparison matrix

Charts must use semantic data tokens.

Examples:

`data.primary`

`data.secondary`

`data.tertiary`

`data.highlight`

`data.positive`

`data.negative`

`data.neutral`

If the client design system lacks enough chart colors, derive an accessible data visualization palette from the approved brand colors.

Do not arbitrarily introduce unrelated colors.

---

# 13. DATA VISUALIZATION COMPONENTS

Every chart should support:

- Title
- Subtitle
- Axis
- Grid
- Labels
- Values
- Legend
- Annotation
- Highlight
- Source
- Date
- Footnote

Do not rely only on color to distinguish data.

Use:

- Labels
- Line styles
- Symbols
- Position
- Patterns where needed

---

# 14. KPI SYSTEM

Create KPI cards for:

- One metric
- Two metrics
- Three metrics
- Four metrics
- Dashboard

Possible client metrics include:

- Revenue
- Leads
- Calls
- Conversions
- Traffic
- Impressions
- Clicks
- Rankings
- Reviews
- Engagement
- Followers
- Reach
- Views
- Cost per lead
- Return on ad spend
- Sales
- Appointments
- Completed jobs
- Average order value
- Customer acquisition cost

Metric components should remain industry independent.

---

# 15. INFOGRAPHIC SYSTEM

Create modular infographic components:

- Header
- Hero stat
- Introduction
- Section
- Numbered step
- Icon step
- Statistic
- Chart
- Quote
- Comparison
- Timeline
- Checklist
- Warning
- Recommendation
- Source
- CTA
- Footer

Support:

- 1080 × 1920
- 1000 × 1500
- 1080 × 1350
- Carousel format

For long content, prefer carousels when readability improves.

---

# 16. CAROUSEL SYSTEM

Create reusable carousel architecture.

## Slide 1

Hook.

## Slide 2

Context.

## Middle Slides

Primary content.

## Penultimate Slide

Summary.

## Final Slide

CTA.

Support:

- Educational
- Case study
- Statistics
- Checklist
- How to
- Mistakes
- Comparison
- FAQ
- Myth versus fact
- Industry commentary
- Data
- Process

Include:

- Page numbering
- Optional swipe indicator
- Persistent branding
- Consistent content area

---

# 17. VIDEO COVER SYSTEM

Create covers for:

- Instagram Reels
- Facebook Reels
- TikTok
- YouTube Shorts reference frames
- Stories

Use the 1080 × 1920 master.

Show safe zones for:

- Platform controls
- Captions
- User information
- Bottom navigation
- Headline
- Logo

Keep key content centered.

---

# 18. YOUTUBE THUMBNAIL SYSTEM

Create dedicated YouTube thumbnail templates.

Support:

- Tutorial
- Case study
- Review
- Reaction
- Commentary
- Comparison
- How to
- Mistakes
- News
- List
- Product
- Service
- Client result

Create composition variants:

- Human focused
- Product focused
- Screenshot focused
- Data focused
- Text focused
- Before and after
- Brand character focused, only when applicable

Rules:

- One dominant idea
- Large focal subject
- Short headline
- High readability
- Minimal small text
- Clear brand recognition

---

# 19. BANNER SYSTEM

Create adaptive banners for:

- Facebook
- Facebook Groups
- LinkedIn
- X
- Bluesky
- YouTube
- Pinterest
- Community pages
- Events
- Podcasts
- Webinars

Each banner should identify:

- Full canvas
- Desktop safe zone
- Mobile safe zone
- Logo area
- Headline area
- Supporting content area
- Optional CTA
- Optional image area

---

# 20. TYPOGRAPHY SYSTEM

Use the active client's typography tokens.

Do not invent another font family.

Create responsive semantic styles for:

- Display
- Eyebrow
- Headline
- Subheadline
- Body
- Statistic
- Quote
- Caption
- Source
- CTA

Adapt type scale by format.

For example:

`social.square.headline`

`social.portrait.headline`

`social.story.headline`

`social.landscape.headline`

`social.banner.headline`

`social.thumbnail.headline`

---

# 21. SPACING

Use the client's existing spacing system.

If a formal spacing system does not exist, derive one from the existing design language before creating templates.

Do not introduce arbitrary spacing values across templates.

---

# 22. GRID SYSTEM

Define grid templates for:

- Square
- Portrait
- Landscape
- Story
- Banner
- Thumbnail
- Infographic

Document:

- Margin
- Columns
- Gutter
- Baseline
- Alignment

---

# 23. PHOTOGRAPHY

Follow the client's existing photography direction.

Respect:

- Lighting
- Framing
- Subject matter
- Color treatment
- Crop
- Depth
- Environment
- Authenticity
- People
- Products
- Equipment

Create reusable image treatments only from styles supported by the brand.

---

# 24. IMAGE CONTAINERS

Build reusable components for:

- Full bleed
- Framed image
- Rounded image
- Cutout subject
- Split image
- Background image
- Screenshot
- Browser frame
- Device frame
- Product image
- Service image
- Portrait

---

# 25. CITATION COMPONENT

Create a reusable source component for statistics and researched content.

Support:

`Source: Organization, Year`

and

`Source: Organization · Report · Year`

The citation must remain readable.

Never fabricate sources.

Never fabricate statistics.

---

# 26. CTA SYSTEM

Derive CTAs from the client's design system.

Support generic actions such as:

- Learn More
- Get Started
- Request Quote
- Book Now
- Call Now
- View Service
- Read More
- Download
- Save
- Share
- Follow
- Contact Us

The template should permit client specific CTA language.

---

# 27. FOOTER SYSTEM

Create:

- Compact footer
- Standard footer
- Expanded footer

Possible elements:

- Logo
- Website
- Handle
- Phone
- CTA
- Source
- Page number
- Copyright

Only display information supplied by the current client system or content.

---

# 28. TEMPLATE STATES

Where appropriate support:

- Light
- Dark
- Image
- Minimal
- Text heavy
- Data heavy
- Brand character
- No brand character
- Product
- Service
- Editorial

Only create states that make sense for the current design system.

---

# 29. COMPONENT ARCHITECTURE

Create reusable components for:

- Logo
- Headline
- Eyebrow
- Body copy
- Statistic
- KPI
- Source
- CTA
- Footer
- Avatar
- Review
- Rating
- Testimonial
- Image
- Icon
- Badge
- Tag
- Browser
- Device
- Chart legend
- Page number
- Carousel indicator
- Comparison
- Quote
- Warning
- Positive state
- Negative state

Use variants rather than duplicate components.

---

# 30. DESIGN TOKENS

Connect every reusable element to design system tokens.

Do not manually enter values repeatedly.

Use variables for:

- Colors
- Text
- Typography
- Spacing
- Radius
- Borders
- Shadows
- Data colors
- Logo assets
- Brand imagery

Changes to the client design system should propagate through the template library whenever possible.

---

# 31. CLIENT SWITCHING MODEL

Design the library so the architecture can be reused for another client.

When switching clients:

1. Load the new client's design system.
2. Replace design tokens.
3. Replace brand assets.
4. Replace typography.
5. Replace imagery rules.
6. Replace optional brand specific components.
7. Preserve the universal content architecture.
8. Review layouts for brand fit.
9. Adjust compositions where the new brand requires it.

Do not manually recolor an old client's social posts and call that a new system.

---

# 32. TEMPLATE NAMING

Use semantic naming.

Examples:

`Social / Feed / Portrait / Statistic`

`Social / Feed / Square / Quote`

`Social / Feed / Landscape / Comparison`

`Social / Story / Statistic`

`Social / Carousel / Cover`

`Social / Carousel / Content`

`Video / Thumbnail / Tutorial`

`Video / Vertical / Cover`

`Banner / YouTube`

`Banner / LinkedIn`

`Data / Bar / Horizontal`

`Data / KPI / Three Metric`

`Infographic / Timeline`

`Component / Citation`

`Component / CTA`

Avoid putting the client name into every component name.

The design file already represents the client.

---

# 33. SAMPLE CONTENT

Do not use Lorem Ipsum.

Generate realistic sample content based on the current client's:

- Industry
- Services
- Products
- Audience
- Geography
- Brand positioning

Sample content should demonstrate real usage without becoming embedded permanently into components.

---

# 34. EDITABILITY

Everything must remain editable.

Use:

- Components
- Variants
- Variables
- Tokens
- Auto layout
- Named text layers
- Named image layers
- Named groups
- Reusable styles

Do not flatten finished templates.

---

# 35. PLATFORM CONFIGURATION

Maintain a central `Platform Specifications` reference.

For every platform list:

- Asset type
- Width
- Height
- Aspect ratio
- Safe zone
- Crop behavior
- Notes

Dimensions change over time.

Do not scatter platform dimensions throughout the design system without a central reference.

When updating a platform specification later, related templates should be easy to locate and revise.

---

# 36. ACCESSIBILITY

Check:

- Text contrast
- Small text
- Color differentiation
- Mobile readability
- Thumbnail readability
- Avatar recognition
- Chart comprehension

Do not communicate important chart differences through color alone.

---

# 37. QUALITY CONTROL

Before marking any template complete, verify:

- Correct dimensions
- Correct active client
- Correct logo
- Correct fonts
- Correct colors
- Correct design tokens
- Correct spacing
- Correct safe zones
- Correct image treatment
- Correct visual hierarchy
- Correct source formatting
- Mobile readability
- No interface collisions
- No incorrect brand assets
- No elements inherited from another client

That last item is especially important.

No asset from a previous client should accidentally survive a client switch.

---

# 38. LIBRARY ORGANIZATION

Organize the finished system into:

1. Foundations
2. Active Client Brand
3. Components
4. Avatars
5. Feed Posts
6. Stories
7. Vertical Video
8. Carousels
9. Banners
10. YouTube
11. Data Visualization
12. Charts
13. KPIs
14. Infographics
15. Reviews
16. Testimonials
17. Case Studies
18. Promotional
19. Educational
20. Announcements
21. Platform Specifications
22. Documentation

---

# 39. DOCUMENTATION

Create a visual documentation section explaining:

- Which design system is active
- How tokens flow into social templates
- Logo usage
- Typography
- Color usage
- Grid
- Spacing
- Image treatment
- Chart system
- Citation system
- Platform safe zones
- Template naming
- Creating new templates
- Updating platform dimensions
- Adding a new content family
- Switching to another client design system

---

# 40. CONTENT REPURPOSING SYSTEM

Document a workflow where ONE source concept can generate a full campaign.

INPUT EXAMPLE:

A client wants to publish a statistic.

GENERATE:

- Square post
- Portrait post
- Landscape post
- Story
- Reel cover
- LinkedIn graphic
- X graphic
- Pinterest graphic
- Google Business Profile graphic
- Carousel
- YouTube Community post
- YouTube thumbnail if applicable

Preserve:

- Message
- Brand
- Hierarchy

Change:

- Composition
- Amount of text
- Cropping
- Scale
- Safe zones

---

# 41. FUTURE CONTENT TYPES

The architecture must make it possible to add future platforms and asset types without redesigning the entire library.

A new platform should mainly require:

1. Canvas specifications
2. Safe zones
3. Crop rules
4. Mapping existing content templates into the new ratio

The underlying brand and content components should remain reusable.

---

# 42. DO NOT DO THIS

Do not:

- Hard code BlakSheep Creative
- Hard code any client
- Carry assets from one client into another
- Assume a mascot exists
- Assume dark backgrounds
- Assume bright colors
- Assume a particular industry
- Create random fonts
- Invent colors
- Modify logos
- Create unrelated visual styles
- Flatten components
- Use Lorem Ipsum
- Shrink one design into every format
- Crop portrait designs into landscape
- Crop landscape designs into portrait
- Ignore safe zones
- Fabricate statistics
- Fabricate citations

---

# 43. SUCCESS CRITERIA

The system is successful when:

A completely different client design system can be loaded and this social template architecture still works.

The resulting graphics should unmistakably belong to THAT CLIENT.

The system should feel like:

**One design system producing many content formats.**

It should never feel like:

**One generic social media template pack with different logos pasted on top.**

The visual architecture should adapt to the client rather than forcing the client into a predetermined visual aesthetic.