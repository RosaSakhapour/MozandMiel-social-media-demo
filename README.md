# MozandMiel-Social-Media-Content-Generator

#### (Source Code Available Upon Request)

An AI-powered social media content generation system I built for my food business, Moz&Miel.

The goal was simple: I wanted to streamline the process of turning a single recipe or video into platform-specific content without manually rewriting everything for each social media platform.

## What It Does

The system takes recipe and content information such as:

* Recipe name and description
* Recipe details and ingredients
* Video context and style
* Main hook or topic
* Personal notes
* Content goals
* Additional instructions

It then uses the OpenAI API to generate tailored content for four platforms:

* **Instagram:** Captions, hooks, calls to action, and hashtags.
* **TikTok:** Short-form video content tailored to the platform.
* **YouTube:** Titles, descriptions, and supporting content for video publishing.
* **Pinterest:** SEO-focused pin titles and descriptions, including multiple variations to experiment with different search-friendly wording.

Each platform has its own content requirements, so the application generates structured outputs tailored to the selected platform rather than treating every post the same way.

## Workflow

Recipe Details and Video Context
↓
Next.js Application
↓
Platform-Specific Prompt Construction
↓
OpenAI API
↓
Structured JSON Output
↓
Response Parsing and Validation
↓
Normalized Platform-Specific Data
↓
Reusable React Components

## Tech Stack

* Next.js
* TypeScript
* React
* Tailwind CSS
* OpenAI API
* Prompt Engineering
* JSON
* JSON Schema
* API Routes
* Data Parsing and Validation
* Git/GitHub
* Cursor AI

## Engineering Highlights

### Platform-Specific Content Generation

Designed prompts and output structures for Instagram, TikTok, YouTube, and Pinterest, accounting for differences in content formats, writing styles, and platform requirements.

### Structured AI Outputs

Used JSON Schema to define the expected shape of generated content, making it easier for the application to work with predictable fields instead of unstructured text.

### TypeScript and Data Handling

Implemented TypeScript utilities to parse generated JSON, handle unexpected value types, normalize incoming data, and prepare content for rendering.

### Reusable React Components

Organized the application into reusable components that separate content input from the presentation of generated results.

### API Integration and Error Handling

Connected the frontend to a Next.js API route for content generation and incorporated handling for AI responses that may not match the expected data structure.

## Why I Built It

Moz&Miel creates educational recipe content across multiple platforms. However, one recipe can require several different pieces of content, each with its own format and audience.

I built this tool to reduce repetitive work and make it easier to adapt my content for each platform.

The project also gave me an opportunity to work hands-on with AI integration, prompt engineering, structured outputs, TypeScript, data validation, and frontend architecture in a real-world application.

Rather than using AI as a simple text generator, I wanted to build a system that could produce structured content that fits into an actual content creation workflow.

## Screenshots

### Content Input Form

<img width="1091" height="668" alt="Screen Shot 2026-10-08 at 7 45 46 PM" src="https://github.com/user-attachments/assets/863209a4-f73b-4281-93f2-fafb8a86edb6" />

### Generated Social Media Content

<img width="1104" height="678" alt="Screen Shot 2026-10-08 at 7 46 05 PM" src="https://github.com/user-attachments/assets/dd9412a2-d8d6-40d9-9aad-03c4b4c98251" />
### Pinterest SEO Variations

## Project Structure

The application is organized around API handling, input components, prompt construction, platform-specific schemas, data validation, and reusable result components.

Key files include:

* `src/app/api/generate-social/route.ts` — handles the social content generation API request.
* `src/components/SocialForm.tsx` — collects recipe information and content instructions.
* `src/components/PlatformResults.tsx` — displays generated social media content.
* `src/lib/build-prompt.ts` — constructs prompts for the selected platforms.
* `src/lib/social-schema.ts` — defines the expected structure of generated content.
* `src/lib/validate-social-content.ts` — parses, validates, and normalizes generated responses.
* `src/lib/types.ts` — defines TypeScript types used throughout the application.

## Future Improvements

* Expand content customization options for different audiences and content goals.
* Improve validation and handling of unexpected AI responses.
* Add more ways to compare and organize content variations.
* Explore integrations that streamline the process of preparing content for publication.

## Note

This repository is a project showcase. Source code is available upon request.
