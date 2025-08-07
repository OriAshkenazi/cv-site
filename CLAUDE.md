# CV Site Design Guidelines & Requirements

## 📋 Project Overview
- **Domain**: cv.oriashkenazi.com
- **Purpose**: Responsive CV for Ori Ashkenazi - Civil Engineer & VDC/BIM Specialist at Shapir LTD
- **Requirements**: Desktop, Mobile, and A4 Print (single page) versions

## 🎨 Color Scheme (Cohesive Yellow/Gold Theme)
- **Body Background**: `linear-gradient(135deg, #fff8e1 0%, #fff3c4 50%, #ffecb3 100%)`
- **Header Background**: `linear-gradient(135deg, #ffd700 0%, #ffeb3b 30%, #ffc107 100%)`
- **Header Text**: Dark gray (`#2d3748`, `#1a202c`) for excellent contrast
- **Accent Colors**: Orange-gold (`#ff8f00`, `#f57c00`) for links and highlights
- **Skill Categories**: `#fffde7` background with `#ffc107` border
- **Experience Hover**: `#ffc107` border with `rgba(255, 193, 7, 0.15)` shadow
- **NO PINKS OR PURPLES**: Removed all non-warm colors for cohesion

## 📐 Typography Hierarchy (Golden Ratio φ = 1.618)
### Desktop Sizes:
- **H1** (Name): `3.236rem` (φ²)
- **H2** (Job Title): `2rem` (φ)
- **H3** (Section Headers): `1.618rem` (φ)
- **H4** (Job Titles): `1.25rem` (φ^0.5)
- **Body Text**: `1rem` (base)
- **Contact Items**: `1.1rem`
- **Expertise Tags**: `0.9rem`

### Mobile Sizes (Much Larger for Readability):
- **H1**: `2.618rem` → `2.2rem` (small screens)
- **H2**: `1.618rem` → `1.414rem` (small screens)  
- **H3**: `1.414rem` → `1.3rem` (small screens)
- **H4**: `1.125rem` → `1.1rem` (small screens)
- **Body Text**: `1.1rem` → `1rem` (small screens)
- **Contact Items**: `1.2rem` → `1.1rem` (small screens)

## 📱 Mobile Layout Requirements
- **Header**: Flexbox column layout, centered text
- **Contact Icons**: 4 items (WhatsApp, Call, Email, LinkedIn) - check spacing
- **Content**: Single column grid
- **Typography**: Much larger than desktop for readability
- **Touch Targets**: Minimum 44px for mobile accessibility

## 📞 Contact Functionality
1. **WhatsApp**: `https://wa.me/972509713042?text=Hi%20Ori,%20I%20saw%20your%20CV%20and%20would%20like%20to%20discuss%20opportunities`
2. **Phone Call**: `tel:+972509713042`
3. **Email**: `mailto:oriashkenazi93+cv@gmail.com?subject=Regarding%20your%20CV`
4. **LinkedIn**: `http://www.linkedin.com/in/ori-ash`

## 🔲 Icon Specifications
- **Size**: All SVG icons 18x18px (uniform square)
- **Color**: Inherit from text color for consistency
- **Style**: Modern, professional, recognizable

## 🖨️ A4 Print Requirements (CRITICAL)
- **Single page constraint**: Must fit on one A4 page
- **No headers/footers**: Use proper `@page` rules
- **Font sizes**: 7.5px-10px range for content density
- **Color**: Black text on white background
- **Layout**: 35% / 65% grid columns
- **Margins**: 0.4in for printable area

## 📦 Container & Layout Rules
- **Desktop**: Centered max-width container with shadows
- **Mobile**: Full-width, no container restrictions
- **Header**: Remove container dependency, use flexbox for balance
- **Spacing**: Even, natural spacing without over-containerization

## 🔄 Cache Busting Strategy
- **CSS Versioning**: `styles.css?v=X.X&parameter=value`
- **Meta Tags**: `no-cache, no-store, must-revalidate`
- **JavaScript Check**: Version detection with forced reload
- **Update Process**: Increment version number with each change

## ⚡ Performance Requirements
- **Fast Loading**: Minimal CSS/JS, optimized assets
- **Responsive Images**: Proper scaling across devices
- **CDN Compatibility**: Works with GitHub Pages, Cloudflare
- **Cross-browser**: Modern browsers + mobile Safari/Chrome

## 🎯 Content Focus
- **Header Focus**: Expertise over company branding
- **Experience**: Shapir LTD as current role (not header)
- **Skills**: VDC Specialist, BIM Expert, Construction Tech
- **All Content**: Preserve original CV information

## 🔧 Technical Requirements
- **Framework**: Vanilla HTML/CSS/JS (no dependencies)
- **Hosting**: GitHub Pages with custom domain
- **SSL**: Automatic HTTPS through GitHub Pages
- **Version Control**: Git with descriptive commits

## 📋 Testing Checklist
- [ ] Desktop responsive (1200px+)
- [ ] Tablet responsive (768px-1199px)  
- [ ] Mobile responsive (320px-767px)
- [ ] A4 print single page
- [ ] Contact links work (WhatsApp, phone, email, LinkedIn)
- [ ] Cache busting effective
- [ ] Cross-browser compatibility
- [ ] Typography hierarchy clear
- [ ] Color scheme cohesive

## 🚨 Common Issues to Avoid
- **Color Clashing**: No pinks, purples, or unrelated colors
- **Mobile Text Too Small**: Always test mobile readability
- **Print Multi-Page**: Must fit single A4 page
- **Cache Problems**: Update version numbers
- **Container Over-Dependency**: Balance structure with flexibility
- **Poor Contrast**: Ensure text readability on backgrounds

## 📈 Future Updates
- Update cache version numbers when making changes
- Test mobile layout when adding new content
- Maintain golden ratio typography relationships
- Keep cohesive color scheme
- Document new decisions in this file