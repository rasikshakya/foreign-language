I worked on making a SPA using Tailwind CSS CDN on the topic Foreign Languages. For this project I used Claude. I first prompted it “Generate a website on Foreign Language. This should be a single page application and use only Tailwind CDN (without using NPM).” Then I iterated it with by making it add JavaScript features. These features included Navbar scroll effect, Scroll Reveal (intersection observer), Language Card Filtering, Flashcard Flip, Quiz Engine and Progress Bar Animation. For this 20+ Tailwind styles were used:

These were used for color and backgrounds:
1.	bg-cream: custom background color #f5f0e8 – a warm off-white defined in tailwind.config
2.	bg-ink: custom near-black #0d0d0d – used for dark sections, navbar and cards
3.	text-gold: custom golden text color #c9933a – used for accents, labels and highlights
4.	bg-gold/15: gold background at 15% opacity – Tailwind’s slash syntax for transparency
5.	bg-white/5: white at 5% opacity – subtle card backgrounds in dark sections
6.	border-white/10: white border at 10% opacity – barely-visible dividers on dark backgrounds

These were used for layout and spacing:
8.	max-w-7xl: Sets max-width: 80rem – constrains content width on wide screens
9.	mx-auto: margin-left: auto; margin-right: auto – centers block elements horizontally
10.	grid md: grid-cols-2: Single column by default, switches to two columns at md (768 px+) breakpoint
11.	gap-6: Sets gap: 1.5rem – spacing between grid or flex children
12.	px-6 md:px-14: Horizontal padding 1.5rem on mobile, 3.5rem on medium+ screens
13.	py-28: Vertical padding 7rem top and bottom – generous section breathing room

These were used for Typography:
15.	font-display: Applies Playfair Display serif font – custom family defined in config
16.	uppercase: Transforms text to ALL CAPS – used on small section labels
17.	italic: Makes text italic – used on hero headline accent words
18.	text-5xl md:text-7xl: Font size 3rem on mobile, scales to 4.5rem on medium+ screens
19.	leading-none: Sets line-height: 1 – tight leading for large display headings
20.	tracking-widest: letter spacing: 0.1rem – wide spacing used on uppercase label/tag text

These were used for Flexbox:
21.	flex items-center justify-between: Row layout, vertically centered, children pushed to opposite ends
22.	flex-wrap: Allows flex children to wrap onto the next line when space runs out
23.	shrink-0: Prevents a flex child from shrinking – keeps icons/flags at their set size
24.	gap-2: gap: 0.5rem between flex children – tight spacing for tags and dot rows

These were used for Transitions & Animations:
23.	transition-all duration-300: Smoothly animates all CSS properties over 300ms
24.	hover:-translate-y-1: On hover, moves the element up by 4px – subtle lift effect on cards
25.	hover:scale-110: Scales element to 110% on hover – used on the logo circle
26.	animate-fade-up: Custom keyframe animation: fades in while sliding up – defined in tailwind.config
27.	animate-pulse: Built-in Tailwind pulse – fades in and out repeatedly, used on status dots

These were used for Borders & Radius:
28.	rounded-full: border-radius: 9999px – perfect pill/circle shape
29.	rounded-2xl: border-radius: 1rem – large rounded corners for cards
30.	border-l-4: Adds a 4px left border only – the colored accent stripe on language cards
31.	border-2: Sets border width to 2px – used on outlined buttons

These were used for Responsive Prefixes:
32.	hidden md:flex: Hidden on mobile (display: none), becomes flex at md (768px+)
33.	md:col-span-2: In a grid, this element spans 2 columns on medium+ screens
34.	sm:grid-cols-2: Switches to a 2-column grid at the sm (640px+) breakpoint
35.	lg:grid-cols-3: Expands to a 3-column grid at lg (1024px+) breakpoint

These were used for Effects & Shadows:
36.	shadow-2xl: Extra-large drop shadow – dramatic depth for the hero card
37.	shadow-lg shadow-gold/25: Large shadow tinted gold at 25% opacity – glowing CTA button effect
38.	blur-3xl: Applies blur(64px) – used on background blobs for soft ambient glow
39.	backdrop-blur-md: Blurs content behind the navbar – frosted glass effect on scroll
40.	overflow-hidden: Clips child elements – used on cards to contain the shine sweep animation
