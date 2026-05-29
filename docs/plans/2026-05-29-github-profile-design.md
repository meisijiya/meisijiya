# GitHub Profile Page Design

## Overview

Design a GitHub Profile page for user `meisijiya` with the following requirements:

### User Information
- **Username**: meisijiya
- **Identity**: Junior (大三) university student
- **Tech Stack**: Java, TypeScript, Python (aspire to master them)
- **Blog**: https://xn--ljhfjm-dl0o.top/
- **Life Philosophy**: 亲疏随缘 (Go with the flow for relationships)
- **Special Message**: "我有个可爱女友，希望我们长长久久，事事顺意，健健康康，开开心心" (I have a lovely girlfriend, hope we last forever, everything goes well, stay healthy and happy)

### Design Requirements
- **Style**: Modern minimalist (similar to Atingaii's profile)
- **Layout**: Centered layout with banner and animated text
- **Components**: 
  - GitHub Stats Card
  - Programming Language Statistics
  - Badges and Links
  - Contribution Streak Statistics
- **Animations**:
  - Typing animation for special message
  - Contribution snake animation
- **Images**: Two K-On! anime images displayed side by side with scrolling effect

### Page Structure

```
┌─────────────────────────────────────────┐
│           Banner Image                  │
│         (Optional background)           │
├─────────────────────────────────────────┤
│         Hi there, I'm meisijiya         │
│    大三在校生 · Java/TS/Python爱好者    │
│          亲疏随缘 · Go with the flow     │
├─────────────────────────────────────────┤
│     [Typing Animation: Special Message] │
├─────────────────────────────────────────┤
│  ┌─────────────────────────────────────┐ │
│  │    K-On! Images (Side by Side)      │ │
│  │    with Scrolling Effect            │ │
│  └─────────────────────────────────────┘ │
├─────────────────────────────────────────┤
│           About Me Section              │
│  - Junior student at university         │
│  - Love Java, TypeScript, Python        │
│  - Blog: https://xn--ljhfjm-dl0o.top/  │
├─────────────────────────────────────────┤
│         Tech Stack & Tools              │
│  ┌─────────────────────────────────────┐ │
│  │ Languages: Java, TS, Python        │ │
│  │ Tools: Git, VS Code, etc.          │ │
│  └─────────────────────────────────────┘ │
├─────────────────────────────────────────┤
│         GitHub Statistics               │
│  ┌──────────────┬──────────────────┐    │
│  │ Stats Card   │ Top Languages    │    │
│  └──────────────┴──────────────────┘    │
│  ┌─────────────────────────────────────┐ │
│  │      Contribution Streak            │ │
│  └─────────────────────────────────────┘ │
├─────────────────────────────────────────┤
│         Badges & Links                  │
│  [Blog] [GitHub] [Email] [Visitors]     │
└─────────────────────────────────────────┘
```

### Implementation Plan

1. **Create Repository**: Create `meisijiya/meisijiya` repository on GitHub
2. **Create README.md**: Implement the profile page structure
3. **Add Components**:
   - GitHub Stats Card via `github-readme-stats`
   - Top Languages via `github-readme-stats`
   - Contribution Streak via `github-readme-streak-stats`
   - Badges via `shields.io`
4. **Add Animations**:
   - Typing animation via `readme-typing-svg`
   - Contribution snake animation via `github-contribution-grid-snake`
5. **Add Images**:
   - Upload K-On! images to repository
   - Implement side-by-side scrolling display
6. **Test and Deploy**: Verify all components work correctly

**Life Philosophy Display**:
- **Text**: 亲疏随缘
- **Translation**: Go with the flow for relationships
- **Position**: Subtitle below the main heading
- **Implementation**: Italic text with a separator (·)

**Banner Design**:
- **Style**: Neon light style "meisijiya" text
- **Implementation**: Create SVG or use text generator
- **Color**: Cyan (#06B6D4) with glow effect
- **Background**: Dark background with gradient
- **Position**: After the "About Me" section
- **Badges**:
  - Blog: https://xn--ljhfjm-dl0o.top/
  - GitHub: https://github.com/meisijiya
  - Visitors counter
- **Implementation**: Horizontal row of badges from shields.io
- **Position**: Below the statistics section
- **Implementation**: GitHub Contribution Grid Snake Animation
- **Service**: `github-contribution-grid-snake` on Vercel
- **Layout**: Side by side for stats card and top languages
- **Implementation**: HTML table or div with flexbox
- **Stats Card**: GitHub Stats Card via `github-readme-stats`
- **Top Languages**: Top Languages via `github-readme-stats`
- **Streak Stats**: Contribution Streak via `github-readme-streak-stats`
- **Snake Animation**: Contribution snake animation below statistics
- **Position**: Below the header, above the images
- **Implementation**: Centered div with typing animation
- **Container**: Full width with centered text
- **Text**: "我有个可爱女友，希望我们长长久久，事事顺意，健健康康，开开心心"
- **Effect**: Character-by-character typing animation
- **Implementation**: Use `readme-typing-svg` service
- **Parameters**:
  - Font: Fira Code or similar monospace font
  - Size: 22px
  - Color: `#06B6D4` (Cyan)
  - Duration: 3200ms per line
  - Pause: 900ms between lines

**Contribution Snake Animation**:
- **Effect**: GitHub contribution grid snake animation
- **Implementation**: Use `github-contribution-grid-snake` service
- **Display**: Below the statistics section

**Image Scrolling Effect**:
- **Effect**: Two K-On! images displayed side by side with horizontal scrolling from right to left
- **Implementation**: Use HTML `<marquee>` tag with `direction="left"` attribute
- **Parameters**:
  - Direction: left (right to left scrolling)
  - Behavior: scroll (continuous scrolling)
  - Scroll amount: 3 (moderate speed)
  - Width: 100% of container
- **Note**: GitHub supports `<marquee>` tag for scrolling effects

### Technical Notes

- **GitHub Profile README**: Must be in a repository named `username/username`
- **Public Repository**: Must be public to display on profile
- **Markdown Support**: GitHub supports most HTML and CSS in README
- **Image Hosting**: Images can be stored in the repository or hosted externally
- **External Services**: Use Vercel-hosted services for stats and animations

**Tech Stack Display**:
- **Format**: Table with categories
- **Categories**:
  - **Languages**: Java, TypeScript, Python
  - **Frameworks**: Spring Boot, Express.js, Flask (example)
  - **Tools**: Git, VS Code, IntelliJ IDEA (example)
  - **Databases**: MySQL, Redis (example)
- **Implementation**: HTML table with badges from shields.io
- **Style**: Flat square badges with logos

Based on user preference:
- **Primary**: `rgb(220, 163, 144)` (Warm pink-brown)
- **Secondary**: `#181717` (GitHub Dark)
- **Accent**: Various badge colors
- **Background**: Transparent or subtle gradient
- **Neon Glow**: Cyan (#06B6D4) for neon text effect

**Blog Address Display**:
- **URL**: https://xn--ljhfjm-dl0o.top/
- **Display Text**: xn--ljhfjm-dl0o.top
- **Implementation**: Badge with blog icon
- **Style**: Flat square badge with blog icon

The profile should look good on:
- Desktop browsers
- Mobile devices (GitHub mobile app)
- Different GitHub themes (light/dark)