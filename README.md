# Chef's Menu Manager 

A React Native mobile application engineered with **Expo Snack** to empower culinary professionals and kitchen managers to effortlessly oversee menu inventories, execute course-based filtering, and track real-time statistics.


## Final POE Submission Overview

* **Module Code:** MAST5112 (Portfolio of Evidence)
* **Application Title:** Chef's Menu Manager
* **Development Environment:** React Native, JavaScript (ES6+), Expo Snack

## Application Navigation & Flow

The system employs a streamlined, state-driven screen architecture ensuring smooth traversal across all operational views:

1. **Home Dashboard:**
   * Exhibits the primary banner and a live total dish counter.
   * Houses primary routing controls for **VIEW MENU**, **ADD NEW DISH**, and **VIEW STATISTICS**.
   
2. **Menu Catalog View:**
   * Reached via the dashboard menu button 
   * Enables keyword searches alongside categorical filters (*All*, *Starter*, *Main*, *Dessert*).
   * Features inline **Edit** and **Delete** buttons for immediate record management.
   * Provides a navigation button back to the home screen 

3. **Dish Entry & Modification Screen:**
   * Accessed through the add or edit action triggers.
   * Collects dish naming, course classification, and pricing data with built-in       validation checks 
   * Includes persistence triggers and a return button to the primary dashboard 

4. **Statistics Dashboard:**
   * Triggered via the statistics navigation button 
   * Calculates real-time total item counts, financial price averages, and category distribution breakdowns.
   * Includes navigation back to the home interface

## Change Log & Version Evolution (Since Part 2)

### 1. Advanced Menu Operations & Feedback
* **Record Modification:** Integrated complete editing capabilities (`handleStartEdit` and `handleAddOrUpdateDish`) enabling updates to dish attributes with immediate interface synchronization.

* **Instant Deletion:** Deployed direct record removal (`handleDelete`) straight from item display cards.

* **Validation & User Alerts:** Implemented strict field validation alongside native feedback alerts confirming successful transactions and error states 

### 2. Search & Categorical Filtering
* **Keyword Matching:** Added real-time text query filters across dish descriptors and classifications.

* **Course Selectors:** Configured quick-action filter buttons for sorting items by culinary course.

* **Case-Insensitive Normalization:** Refined filter algorithms to guarantee precise category matching regardless of text casing.

### 3. Analytics & Statistics Suite
* Deployed a dedicated analytics view providing live computational metrics:
  * **Aggregate Volume:** Dynamic tracking of total active menu items.
  * **Mean Pricing:** Automated calculation of average menu pricing (`R 0.00`).
  * **Category Distribution:** Specific item counts grouped by course type.

## Refactoring Highlights

* **Modular Code Organization:** Consolidated state hooks, handler logic, routing switches, and visual layouts into a clean, unified structure optimized for Expo Snack

* **Design Consistency:** Standardized color tokens (`#5BC0DE` primary theme, `#428BCA` accents, `#D3D3D3` containers) and padding metrics across all view screens to ensure a cohesive look and feel

* **Semantic Naming Conventions:** Adopted explicit identifiers for functions (`handleStartEdit`, `handleDelete`) and state collections (`filteredItems`, `averagePrice`) to maximize code readability

* **State Management Efficiency:** Optimized component state hooks to ensure calculations update dynamically without demanding manual page refreshes.

## Execution Guide

1. Launch the project source within **Expo Snack**.
2. Test functionality via the web runner or scan the active QR code using the **Expo Go** mobile application.

3. Utilize the dashboard navigation to evaluate:
   * **Menu Management:** Search, filter, modify, and remove dishes.
   * **Data Entry:** Verify input validation controls.
   * **Statistics:** Review live pricing and category metrics.

## Final Submission Checklist

- All required core and enhanced features fully implemented 
- Codebase refactored for readability, consistent layout, and clean architecture
- Comprehensive README.md incorporating change logs and refactoring note
- Source code published to designated GitHub repository
- Video demonstration recording linked for assessment
