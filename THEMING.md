# Puppy Breeder Website Theming Guide

Use this guide to re-theme this template for any dog breed. Copy the prompt at the bottom to quickly re-theme for a new breed.

---

## Site Structure

```
/
├── index.html              # Homepage (hero, puppies, about, blog, testimonials, contact)
├── available-puppies.html  # Detailed puppy listings page
├── about.html              # About the breeder story
├── about-breed.html        # Breed-specific information (size, temperament, care)
├── contact.html            # Contact form page
├── reviews.html            # Customer testimonials
├── basic-care.html         # Puppy care guide
├── faqs.html               # Frequently asked questions
├── health-guarantee.html   # Health guarantee policy
├── pickup-delivery.html    # Pickup and delivery info
├── privacy-policy.html     # Privacy policy
├── return-refund.html      # Return/refund policy
├── sales-agreement.html    # Sales agreement form
├── vaccinations.html       # Vaccination schedule
├── thank-you.html          # Form submission confirmation
├── style.css               # All styles and color variables
├── script.js               # JavaScript functionality
└── public/images/          # Puppy photos (8 images)
```

---

## What To Change For Each Theme

### 1. Brand Identity
| Element | Location | Example |
|---------|----------|---------|
| Business Name | All HTML files (navbar, footer, forms) | "Merry Muzzle Pets" |
| Logo Initials | All HTML files (`.logo` div) | "MM" |
| Email Address | All HTML files (mailto links, contact info) | info@merrymuzzlepets.com |
| Website URL | All HTML files (SMS links, footer) | Merrymuzzlepets.com |
| Form Subject Lines | Hidden form inputs | "Merry Muzzle Pets Contact Form" |

### 2. Color Scheme (style.css :root variables)
```css
:root {
    --primary: #0891b2;           /* Main brand color (buttons, links, accents) */
    --primary-dark: #0e7490;      /* Darker shade for hover states */
    --accent: #fb923c;            /* Secondary accent color */

    /* Background tones - should complement primary */
    --cream: #f0fdfa;
    --soft-cream: #f5fffe;
    --surface-soft: #f0fdfa;
    --surface-tint: #ecfeff;
    --gradient-rose: #e0f7fa;
    --gradient-warm-start: #ecfeff;
    --gradient-warm-mid: #f0fdfa;
    --bg-warm: #f5fffe;
    --table-header: #e0f7fa;
    --table-total: #f0fdfa;
    --text-highlight: #e0f7fa;
}
```

#### Suggested Color Palettes by Breed Type

| Breed Type | Primary | Primary Dark | Accent | Background Tint |
|------------|---------|--------------|--------|-----------------|
| **French Bulldog** (playful) | #0891b2 (teal) | #0e7490 | #fb923c (orange) | #f0fdfa |
| **Dobermann** (bold) | #ca0f48 (crimson) | #a30c3a | #f5b63f (gold) | #fff4e6 |
| **Golden Retriever** (warm) | #d97706 (amber) | #b45309 | #059669 (green) | #fffbeb |
| **German Shepherd** (strong) | #374151 (slate) | #1f2937 | #dc2626 (red) | #f9fafb |
| **Poodle** (elegant) | #7c3aed (purple) | #6d28d9 | #ec4899 (pink) | #faf5ff |
| **Labrador** (friendly) | #2563eb (blue) | #1d4ed8 | #f59e0b (yellow) | #eff6ff |
| **Husky** (cool) | #0ea5e9 (sky) | #0284c7 | #64748b (gray) | #f0f9ff |
| **Bulldog** (sturdy) | #854d0e (brown) | #713f12 | #ca8a04 (gold) | #fefce8 |

### 3. Hardcoded Colors to Update (style.css)
These colors are hardcoded and need manual updates:
- `.badge` background
- `.pill` background
- `.status-pill` background (rgba value)
- `.price-tag` background
- `.blog-date` background
- `.features` section background
- `.blog` section background
- `.stat-card` background

### 4. Puppy Listings
Each site needs **8 puppies** with:
- **Name** (unique, breed-appropriate)
- **Gender** (Male/Female)
- **Image** (placed in `public/images/`)
- **Age** (typically 8-12 weeks)
- **Temperament** (2-3 word description)
- **Description** (1-2 sentences about personality)

**Files to update:**
- `index.html` - Puppy grid section + contact form checkboxes
- `available-puppies.html` - Detailed puppy cards
- `contact.html` - Puppy checkboxes
- `reviews.html` - Puppy names in testimonials

### 5. Breed-Specific Content (about-breed.html)
Update these breed stats:
- **Temperament** (e.g., "Affectionate, playful, adaptable")
- **Energy Level** (Low/Moderate/High + description)
- **Ideal Home** (apartment-friendly? yard needed?)
- **Coat & Care** (shedding level, grooming needs)
- **Adult Size** (weight range, height at shoulder)
- **Lifespan** (typical years)
- **Health Priorities** (breed-specific health concerns)
- **Training Tips** (breed-specific training advice)

### 6. Images Required
Place in `public/images/` folder:
```
[Puppy1 Name] [gender] [breed].jpg
[Puppy2 Name] [gender] [breed].jpg
... (8 total puppy images)
```

**Image naming convention:** `"Buddy male French bull dog.jpg"`

### 7. Hero Section Images (index.html)
Three images in the hero:
- Main large image
- Top circle image
- Bottom circle image

---

## Quick Theme Checklist

- [ ] Update `style.css` color variables
- [ ] Update hardcoded color values in `style.css`
- [ ] Replace brand name in all HTML files
- [ ] Replace logo initials (NW, MM, etc.)
- [ ] Update email addresses
- [ ] Update website URLs in SMS links
- [ ] Update form hidden field subjects
- [ ] Add 8 puppy images to `public/images/`
- [ ] Update puppy listings in `index.html`
- [ ] Update puppy listings in `available-puppies.html`
- [ ] Update puppy checkboxes in `index.html` contact form
- [ ] Update puppy checkboxes in `contact.html`
- [ ] Update breed info in `about-breed.html`
- [ ] Update reviews with new puppy names
- [ ] Update hero images in `index.html`
- [ ] Update about section image

---

## Re-Theming Prompt

Copy and customize this prompt to request a new theme:

```
Please re-theme this puppy breeder website template for [BREED NAME].

## Brand Details
- Business Name: [YOUR BUSINESS NAME]
- Website: [yourwebsite.com]
- Email: [info@yourwebsite.com]

## Color Preference
[Choose one: warm/cool/bold/elegant/natural OR specify colors]

## Puppies (8 total)
Provide names and genders:
1. [Name] - [Male/Female]
2. [Name] - [Male/Female]
3. [Name] - [Male/Female]
4. [Name] - [Male/Female]
5. [Name] - [Male/Female]
6. [Name] - [Male/Female]
7. [Name] - [Male/Female]
8. [Name] - [Male/Female]

## Images
I have placed 8 puppy images in public/images/ named:
[List your image filenames]

## Instructions
- Read the theming.md file for guidance
- Update color scheme in style.css
- Update all brand references across HTML files
- Update puppy listings with my puppies
- Update about-breed.html with accurate [BREED NAME] information
- Keep the site structure intact - only update colors and content
```

---

## Example Completed Prompt

```
Please re-theme this puppy breeder website template for Golden Retrievers.

## Brand Details
- Business Name: Sunny Paws Goldens
- Website: sunnypawsgoldens.com
- Email: info@sunnypawsgoldens.com

## Color Preference
Warm and friendly - amber/gold primary with green accents

## Puppies (8 total)
1. Biscuit - Male
2. Honey - Female
3. Murphy - Male
4. Daisy - Female
5. Cooper - Male
6. Bella - Female
7. Tucker - Male
8. Luna - Female

## Images
I have placed 8 puppy images in public/images/ named:
- Biscuit male Golden Retriever.jpg
- Honey female Golden Retriever.jpg
- Murphy male Golden Retriever.jpg
- Daisy female Golden Retriever.jpg
- Cooper male Golden Retriever.jpg
- Bella female Golden Retriever.jpg
- Tucker male Golden Retriever.jpg
- Luna female Golden Retriever.jpg

## Instructions
- Read the theming.md file for guidance
- Update color scheme in style.css
- Update all brand references across HTML files
- Update puppy listings with my puppies
- Update about-breed.html with accurate Golden Retriever information
- Keep the site structure intact - only update colors and content
```

---

## Files Changed During Theming

For reference, a complete re-theme typically modifies these files:
1. `style.css` - Color variables and hardcoded colors
2. `index.html` - Everything
3. `available-puppies.html` - Puppy listings
4. `about.html` - Brand name, images
5. `about-breed.html` - All breed-specific content
6. `contact.html` - Brand, puppy checkboxes
7. `reviews.html` - Brand, puppy names in reviews
8. `basic-care.html` - Brand, breed references
9. `faqs.html` - Brand, breed references
10. `health-guarantee.html` - Brand
11. `pickup-delivery.html` - Brand
12. `privacy-policy.html` - Brand
13. `return-refund.html` - Brand
14. `sales-agreement.html` - Brand
15. `vaccinations.html` - Brand
16. `thank-you.html` - Brand

---

## Bulk Replace Commands (Optional)

For quick brand name replacement across all files:
```bash
# Replace business name
sed -i '' 's/Old Business Name/New Business Name/g' *.html

# Replace logo initials
sed -i '' 's/>OB<\/div>/>NB<\/div>/g' *.html

# Replace email
sed -i '' 's/old@email.com/new@email.com/g' *.html

# Replace website
sed -i '' 's/oldwebsite.com/newwebsite.com/g' *.html

# Replace breed name
sed -i '' 's/Old Breed/New Breed/g' *.html
```

Then manually update:
- Puppy images and listings
- Breed-specific content in about-breed.html
- Color scheme in style.css
