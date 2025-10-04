---
type: documentation
purpose: tagging-strategy
tags: [meta, organization, tagging, obsidian]
---

# Tagging Strategy for ENG 1181

## 🎯 Overview
This document outlines the comprehensive tagging strategy for organizing course content and optimizing knowledge discovery in Obsidian.

## 📊 Tag Hierarchy & Categories

### 1. **Subject Tags** (Primary Classification)
- `#electricity` - All electrical engineering concepts
- `#matlab` - MATLAB programming and applications
- `#engineering` - General engineering principles
- `#mathematics` - Mathematical concepts and formulas

### 2. **Topic Tags** (Secondary Classification)
- `#resistors` `#capacitors` `#voltage` `#current` `#resistance`
- `#ohms-law` `#kirchhoff` `#circuits` `#voltage-divider`
- `#arrays` `#loops` `#functions` `#variables` `#plotting`
- `#scripts` `#input-output` `#formatting` `#debugging`

### 3. **Difficulty Tags** (Learning Progression)
- `#fundamental` - Basic concepts everyone must know
- `#intermediate` - Concepts requiring some foundation
- `#advanced` - Complex topics requiring mastery of fundamentals
- `#expert` - Highly specialized or complex applications

### 4. **Content Type Tags**
- `#concept` - Theoretical knowledge and definitions
- `#formula` `#calculation` - Mathematical formulas and calculations
- `#practice` `#problem` - Practice problems and exercises
- `#example` - Worked examples and demonstrations
- `#lab` - Laboratory procedures and experiments
- `#reference` - Quick reference materials

### 5. **Course Structure Tags**
- `#eng1181` - Course identifier
- `#week1` `#week2` etc. - Temporal organization
- `#exam1` `#exam2` `#final` - Exam preparation
- `#assignment` `#homework` - Assignment-related content

### 6. **Status Tags** (Progress Tracking)
- `#mastered` - Fully understood and practiced
- `#learning` - Currently studying
- `#review` - Needs additional review
- `#confused` - Requires clarification or help

### 7. **Application Tags**
- `#circuit-analysis` - Circuit analysis applications
- `#data-analysis` - Data processing and analysis
- `#problem-solving` - General problem-solving techniques
- `#real-world` - Real-world applications

## 🎨 Tagging Best Practices

### YAML Frontmatter (Structured Tags)
```yaml
---
concept: ohms-law
topic: basic-electricity
difficulty: fundamental
tags: [electricity, ohms-law, voltage, current, resistance, formulas]
status: mastered
week: 2
---
```

### Inline Tags (Quick Access)
Use inline tags at the end of notes for quick filtering:
```markdown
#electricity #ohms-law #formulas #fundamental #eng1181
```

### Combination Strategy
- **Use both frontmatter AND inline tags**
- Frontmatter for structured searches and metadata
- Inline tags for quick visual scanning and graph view

## 🔍 Search Patterns

### Find All Fundamental Electricity Concepts
```
tag:#electricity AND tag:#fundamental
```

### Find All MATLAB Practice Problems
```
tag:#matlab AND tag:#practice
```

### Find Content Needing Review
```
tag:#review OR tag:#confused
```

### Find Exam Preparation Material
```
tag:#exam1 OR tag:#exam2 OR tag:#final
```

## 📈 Tag Usage Guidelines

### 1. **Consistency Rules**
- Always use lowercase for tags
- Use hyphens for multi-word tags (`#ohms-law` not `#ohms law`)
- Be specific but not overly granular

### 2. **Quantity Guidelines**
- **3-6 tags per note** for optimal discoverability
- Include at least one subject tag and one difficulty tag
- Add status tags for active learning tracking

### 3. **Evolution Strategy**
- Start with core tags, add specialized ones as needed
- Review and refine tags monthly
- Archive unused tags to prevent clutter

## 🎯 Templates Integration

### Concept Note Template
```yaml
---
concept: {{concept-name}}
topic: {{topic-area}}
difficulty: {{fundamental|intermediate|advanced|expert}}
tags: [{{subject}}, {{concept-name}}, {{related-tags}}]
status: learning
week: {{week-number}}
---
```

### Practice Problem Template
```yaml
---
type: practice-problem
topic: {{topic-area}}
difficulty: {{level}}
tags: [{{subject}}, practice, problem, {{specific-tags}}]
status: learning
---
```

## 🔗 Integration with Course Structure

### MOC Organization
- Use tag clouds in MOCs for visual organization
- Group related tags in sections
- Provide tag-based navigation

### Dashboard Integration
- Create tag-based progress tracking
- Use tag queries for automatic content discovery
- Link tags to study schedules

## 📊 Success Metrics

### Effective Tagging Indicators
- [ ] Can find any concept in under 30 seconds
- [ ] Tags accurately reflect content difficulty
- [ ] Status tags align with actual understanding
- [ ] No orphaned or unused tags

### Monthly Review Checklist
- [ ] Review tag usage statistics
- [ ] Update status tags based on understanding
- [ ] Consolidate similar or redundant tags
- [ ] Add missing tags to untagged content