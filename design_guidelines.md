# E-Commerce Design Guidelines

## Design Approach

**Reference-Based Approach:** Drawing inspiration from modern e-commerce leaders (Shopify storefronts, Etsy, contemporary DTC brands) combined with local store warmth and community feel. Focus on clean product presentation, intuitive shopping flows, and building trust through professional polish.

**Core Principles:**
- Product-first visual hierarchy
- Seamless shopping experience with minimal friction
- Professional credibility balanced with approachable personality
- Mobile-optimized for on-the-go shopping

## Typography

**Font Stack (Google Fonts):**
- Primary: Inter (clean, modern sans-serif for UI and body text)
- Accent: Playfair Display (elegant serif for store name and special headings)

**Type Scale:**
- Hero heading: 3xl-5xl, font-bold
- Section headings: 2xl-3xl, font-semibold
- Product names: lg-xl, font-medium
- Body text: base, font-normal
- Prices: lg-xl, font-bold
- Labels/metadata: sm, font-medium

## Layout System

**Spacing Primitives:** Tailwind units of 2, 4, 6, 8, 12, 16
- Component padding: p-4, p-6, p-8
- Section spacing: py-12, py-16, py-20
- Grid gaps: gap-4, gap-6, gap-8
- Element margins: m-2, m-4, m-6

**Container Strategy:**
- Max-width: max-w-7xl for main content
- Product grids: max-w-7xl
- Checkout flow: max-w-4xl (focused, distraction-free)

## Component Library

### Navigation
**Header:** Sticky navigation with store logo (left), category links (center), search bar, cart icon with item count badge, account icon (right). Height: h-16 to h-20. Include trust indicator text below main nav: "Free shipping over $50 • Secure checkout"

### Hero Section
Full-width banner (h-96 to h-screen on desktop, h-64 on mobile) featuring lifestyle product photography showcasing store's personality. Overlay with store tagline and primary CTA ("Shop Now" button with blurred background). Include secondary text highlighting value prop ("Supporting local since [year]" or "Handpicked quality products").

### Product Grid
**Layout:** 
- Desktop: 4 columns (grid-cols-4)
- Tablet: 3 columns (grid-cols-3)
- Mobile: 2 columns (grid-cols-2)

**Product Card Structure:**
- Aspect ratio image container (square or 4:3)
- Product name (truncate to 2 lines)
- Price (prominent)
- Rating stars with review count
- "Add to Cart" button (appears on hover on desktop, always visible on mobile)
- "Quick View" icon button
- Sale badge if applicable (top-right corner)

### Product Detail Page
**Two-column layout (desktop):**
- Left (60%): Large product image with thumbnail gallery below
- Right (40%): Product name, price, star rating with review count, short description, size/variant selector (if applicable), quantity selector, "Add to Cart" + "Buy Now" buttons stacked, trust badges (secure checkout, return policy), accordion sections (full description, shipping info, reviews)

### Shopping Cart
**Slide-out panel (desktop) or full page (mobile):**
- Header with "Shopping Cart" title and close icon
- Line items: product image (thumbnail), name, variant, quantity adjuster (+/-), price, remove button
- Subtotal calculation
- "Continue Shopping" link
- "Proceed to Checkout" button (sticky at bottom)
- Free shipping progress bar ("Add $X more for free shipping")

### Checkout Flow
**Three-step process with progress indicator:**
1. Shipping Information
2. Payment Details
3. Order Review

Clean, single-column form layout. Each section in card with header. Include order summary sidebar (desktop) or expandable summary (mobile) showing cart items and totals.

### Filtering & Sorting Sidebar
**Left sidebar (desktop) or drawer (mobile):**
- Category checkboxes
- Price range slider
- Brand/Material filters (checkboxes)
- Rating filter
- "Clear All Filters" link
- Sort dropdown at top: "Sort by: Featured, Price: Low to High, Price: High to Low, Newest, Best Selling"

### Product Reviews Section
Star rating summary with visual bar chart showing rating distribution. Individual review cards with reviewer name, verified purchase badge, star rating, date, review text, helpful votes.

### Footer
**Multi-column layout:**
- Column 1: Store logo, brief description, social media icons
- Column 2: Shop (category links)
- Column 3: Support (Contact, FAQ, Shipping, Returns)
- Column 4: Newsletter signup (email input + subscribe button)
- Bottom bar: Copyright, payment method icons, trust badges

### Additional Components
- **Category Cards:** Featured categories with image backgrounds and overlay text (3-column grid)
- **Featured Products Carousel:** Horizontal scroll of product cards
- **Order Confirmation Page:** Large checkmark icon, order number, customer details recap, items ordered, shipping info, CTA to continue shopping
- **Search Results:** Same product grid with search term highlight and result count

## Images

**Hero Section:**
Large, high-quality lifestyle image showing products in context or store atmosphere. Could be: curated product flat-lay, store interior with products, satisfied customer using product, or seasonal/thematic scene. Image should evoke the store's personality (artisan, modern, family-friendly, etc.).

**Product Images:**
Clean, well-lit product photography on white/neutral backgrounds for grid view. Detail page should include multiple angles and lifestyle shots showing product in use.

**Category Cards:**
Styled images representing each category with subtle overlay for text readability.

**Trust Elements:**
Consider adding: team photo in About section, store exterior photo, behind-the-scenes shots to build local connection.

## Icons
**Heroicons** (via CDN) for all UI icons: shopping cart, search, user account, chevrons, filters, heart (wishlist), star ratings, check marks.