# Team Section Editing Guide

## How to Edit Team Members

The team section is located in `about.html` between the comments:
```html
<!-- TEAM SECTION - EDITABLE -->
...
<!-- END TEAM SECTION -->
```

## To Add/Edit a Team Member:

### 1. Find the Team Card in about.html
Each team member has this structure:

```html
<div class="team-card">
    <div class="team-image">
        <img src="images/team/member1.jpg" alt="Name Here">
        <div class="team-overlay"></div>
    </div>
    <div class="team-info">
        <h3>Name Here</h3>
        <p class="team-bio">Bio description here...</p>
        <ul class="team-details">
            <li><strong>Subject:</strong> Subject Name</li>
            <li><strong>Experience:</strong> X+ years</li>
        </ul>
    </div>
</div>
```

### 2. What to Edit:

**Image:**
- Save team member photo in `images/team/` folder
- Name it: `member1.jpg`, `member2.jpg`, etc.
- Update the `src` attribute: `src="images/team/yourfilename.jpg"`
- Update the `alt` attribute: `alt="Team Member Name"`

**Name:**
- Change the text in `<h3>Name Here</h3>`

**Bio:**
- Change the text in `<p class="team-bio">...</p>`

**Details:**
- Update Subject: `<li><strong>Subject:</strong> Your Subject</li>`
- Update Experience: `<li><strong>Experience:</strong> X+ years</li>`

### 3. To Add More Team Members:

Copy the entire `<div class="team-card">...</div>` block and paste it before the closing `</div>` of `team-grid`.

### 4. To Remove a Team Member:

Delete the entire `<div class="team-card">...</div>` block for that member.

## Image Requirements:

- **Format:** JPG or PNG
- **Recommended Size:** 400x500 pixels (portrait orientation)
- **Location:** Save in `images/team/` folder
- **Naming:** member1.jpg, member2.jpg, member3.jpg, etc.

## Example Edit:

**Before:**
```html
<h3>Alex Braun</h3>
<p class="team-bio">An experienced teacher...</p>
<li><strong>Subject:</strong> Math</li>
```

**After:**
```html
<h3>John Doe</h3>
<p class="team-bio">A passionate educator who loves teaching physics...</p>
<li><strong>Subject:</strong> Physics</li>
```

## Tips:

- Keep bios concise (2-3 sentences)
- Use consistent image sizes for best appearance
- The grid automatically adjusts to fit 1-4 members per row
- Cards have hover effects built-in (no extra code needed)
