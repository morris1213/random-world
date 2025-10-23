# Random Information Generator

## Overview

This project is a multi-country information generator that provides users with randomly generated, realistic-looking personal information. It is designed as a simple and efficient tool for developers, testers, and anyone needing mock data for different locales. The interface is designed to be modern, intuitive, and visually appealing.

## Project Outline: Style, Design, and Features

### Core Functionality
*   **Immediate Data on Load:** The application automatically generates and displays a set of random information as soon as the page loads, providing immediate value to the user.
*   **Multi-Country Random Data Generation:** Generates a complete set of personal data with one click. Users can select the desired country before generation.
    *   **Supported Countries:** United States, United Kingdom, Canada, Australia, Germany, Japan.
    *   **Common Data:** Full Name, Job Title, Phone Number, Credit Card Information, and a realistic **Email Address** generated from a list of common and country-specific domains.
    *   **Country-Specific Data:** Includes unique address formats and national identifiers for each country (e.g., SSN, NINO, SIN, TFN, etc.).
*   **One-Click Copy:** A convenient button to copy all generated information to the clipboard.

### Visual Design & Aesthetics
*   **Modern UI:** A clean, card-based layout for displaying information.
*   **Branding:** The application's title is consistently set to "Random Information Generator."
*   **Country Selector:** A styled dropdown menu for easy country switching.
*   **Bold Definition:**
    *   **Color Palette:** A vibrant, energetic look with glowing effects.
    *   **Typography:** Expressive and hierarchical font sizes.
    *   **Texture:** A subtle noise texture on the background.
    *   **Visual Effects:** "Lifted" cards with soft, deep drop shadows.
    *   **Iconography:** Modern icons for enhanced user understanding.
    *   **Interactivity:** A glowing, responsive "Generate" button.

### Architecture
*   **Framework:** Built with Astro.js for a fast, static-first experience.
*   **Component-Based:** Core logic is in a single, client-side interactive Astro component (`Generator.astro`).
*   **Client-Side Logic:** All data generation is handled in JavaScript, organized into an easily extensible `countryData` object.
*   **Styling:** In-component scoped CSS using modern features.

## Current Task: Initial Data on Load

**Status: Completed**

The user experience was improved by providing immediate feedback on page load.

*   **Feature Implementation:** The component now automatically calls the `generateData()` function when the page's DOM is fully loaded.
*   **UI Update:** The initial placeholder text ("Select a country...") was removed, as the results card is now populated with data from the start.
*   **Documentation:** Updated this `blueprint.md` file to reflect the new functionality.
