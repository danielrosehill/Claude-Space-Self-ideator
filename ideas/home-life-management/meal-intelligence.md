---
name: "Meal Intelligence"
category: "home-life-management"
description: "Meal planning, recipe management, and grocery optimization"
duration: "ongoing"
difficulty: "medium"
---

# Meal Intelligence

## Use Case

Meal planning, recipe management, grocery optimization, and nutrition tracking in one integrated workspace. Reduce the cognitive load of "what's for dinner" while eating better and wasting less.

## Execution Difficulty

**Level**: Medium

**Rationale**: Multiple interconnected workflows (recipes, planning, shopping, nutrition) but each is well-defined.

## Suggested Folder Structure

```
├── recipes/
│   ├── favorites/
│   ├── to-try/
│   └── by-type/
├── meal-plans/
│   ├── templates/               # Reusable plans
│   └── weekly/                  # Weekly plans
├── inventory/
│   ├── pantry.md
│   └── expiring.md              # Items expiring soon
├── shopping/
│   └── lists/                   # Generated shopping lists
└── outputs/
    └── nutrition-reports/       # Nutrition analysis
```

## Key Workflows

- Build and organize recipe library with tags and ratings
- Generate weekly meal plans based on preferences and inventory
- Create optimized shopping lists from meal plans
- Track pantry inventory and flag expiring items
- Analyze nutritional patterns over time

## Suggested Slash Commands

| Command | Purpose |
|---------|---------|
| `/plan-week` | Generate meal plan for coming week |
| `/generate-list` | Create shopping list from meal plan |
| `/use-inventory` | Suggest meals using items on hand |
| `/add-recipe` | Add and categorize new recipe |

## Suggested Agents

| Agent | Role |
|-------|------|
| `meal-planner` | Generates balanced, varied meal plans based on constraints |

## Why This Works as a Claude Space

- Recipe library grows into personalized resource
- Meal planning benefits from knowing past patterns
- Inventory tracking reduces food waste
