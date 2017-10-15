# Summary of "Localization Essentials"

Course website: https://classroom.udacity.com/courses/ud610

## Lesson 1: Key concepts

- Why is localization important
- Software companies have "internationalization" teams
- uses the Google Fit as an example

## Language of localization (key terms used in localization)

- Globalization (g11n)
    - "Globalization is a marketing strategy to do business in and offer products in international markets."
    - “Globalization addresses the business issues associated with taking a product global. In the globalization of high-tech products this involves integrating localization throughout a company, after proper internationalization and product design, as well as marketing, sales, and support in the world market. (LISA definition, cit. Esselink 2000: 4)”
- Internationalization (i18n)
    - “Internationalization is the process of generalizing a product so that it can handle multiple languages and cultural conventions without the need for re-design. (LISA definition, cit. Esselink 2000: 2)”
    - Examples
        - character encoding
        - date and time formats
- Localization (l10n)
    - “Localization involves taking a product and making it linguistically and culturally appropriate to the target locale (country/region and language) where it will be used and sold. (cit. Esselink 2000: 3)”
    - Involves not only text but also "adapting date and time formats, changing currencies, cultural appropriation, changing the design and the way user experience a product and complying with local laws and regulations"
- Translation (t9n)
- Locale
    - "the linguistic, cultural and other requirements of a specific target market"

## Useful resource

- [Glossary for localization from Google](https://classroom.udacity.com/courses/ud610/lessons/3392b96c-d1bc-429f-afd9-54a50847d89d/concepts/54198b6f-8545-4d5a-b034-40b6ac759d2d)

## Lesson 2: Content types

- Ask the following questions
    1. Where? 
    2. Who? 
    3. Why?
- Marketing content
    - e.g.: website landing page    
    - goal is to be persuasive
    - Requires
        - high local sensitivity
        - high creativity
            - consider rewriting taglines from scratch
            - distance yourself from literal translations to engage potential users
- Online help
    - FAQs, software docs, troubleshooting manuals
    - Challenges
        - product knowledge
        - consistent terminology
- Audio-visual content (subtitling and voiceover)
    - e.g. Google Fit has a video for developers for APIs
    - Why?
        - delivers message faster and more effectively than text
        - more user engagement than text
    - Challenge
        - how? 
            - revoicing
                - dubbing is the most common
            - subtitles
                - two lines, centered
                - limits: 35-45 characters per line
                - less cost than dubbing
        - Consider target audience and number of languages
- User interface
    - 3 common types of software
        - desktop applications
        - web apps 
        - mobile apps
    - Challenges
        - lack of context for translators
            - limited space
        - lack of product knowledge
            - important to ensure proper information exchange
                - include message descriptions for strings to help translators
                    - provides important context
                - e.g. software Google Translator Toolkit 
                - product teams should provide reference material and guidelines
                    - screenshots, string descriptions, demos, mocks
                    - style guides
                    - character limmits
                    - provide a channel of communication between product team and translators
- SEO (search engine optimization), SEM
    - organic search results vs search ads
    - SEM (search engine marketing) = SEO + search ads
    - SEO: what keywords might users use? and include them in the website content
    - Challenge
        - local relavance
            - search words vary greatly by locale
            - learn trends for target markets
            - review keywords used by competitors
            - e.g. Google's keyword tool

## Lesson 3: Profiles and skills

- Profiles and roles in localization at Google
    - Product team 
    - localization team 
        - localization production
        - language services
        - localization operations
            - technology
                - technical operations manager
            - business
        - vendor operations
    - localization project manager (LPM) 
    - language service providers (LSP) 
    - language manager (1 person per language)
        - works on terminology
        - works on naming with product team
        - truncation issues

## Lesson 4: Processes

1. Product preparation
    - done by requester (product team)
    - market insights
    - must analyze local markets
        - group by order of importance
        - language tiering (how important the language is)
    - internationalization (happens during software development)
        - product must be designed for the target markets and cultures
        - Google has an internationalization team
        - Steps for internationalization
            - 1. Design and engineering
            - Considerations:
                - Density and fonts
                - layout 
                - images: no text in images
                - colors: different meanings for different cultures
                - spacing: text expansion, UI buttons need to be made to expand (or have clear character limits)
                - every piece of text should be accompanied by a message description
                - dates, currencies, units, phone numbers
                    - use tools such as internationalization libraries to automate
                    - https://developers.google.com/international/
                - plurals and genders
                    - use international components for unicode to automate
                    - http://site.icu-project.org/
            - 2. Testing
                - pseudolocalization
                - problems
                    - length of text
                    - direction of text
                    - untranslated text
                    - not enough space (truncation)
                    - improperly mirrored interface (e.g. Hebrew, right-to-left)
2. Project preparation
    - Quote (time and cost)
        - overview
        - estimated number of words
        - deliverables
        - deadlines
        - costs
    - Create a localization kit to send out to translators
        - content to be translated
        - terminology
            - Glossary
            - contains the term that are commonly used in the project and that need to be consistent throughout
        - style guide
        - translation memory
        - reference material
3. Project execution
    - Translate (translators
        - use translation tools
    - Review by another LSP (reviewers)
        - verify quality
        - use "quality evaluation tools"
    - Language managers
        - set overall language standards
        - facilitate between translation and review teams
4. Quality assessment (QA)
    - Final check on the whole product 
        - not limited to only the text
    - Steps
        1. automated quality assurance
            - uses automated tools
        2. Linguistic quality testing + functional quality testing
            - requires collaboration with engineers, designers, testers, translators
    - Test plan
        - created by product team engineers
        - communication channel with reviewers and engineers

## Lesson 5: Tools

- Project preparation stage
    - Localization project management tools
        - Translation management tools
        - Terminology management tools
            - termbases
        - Translation memory management tools
- Project execution stage
    - Computer-aided translation (CAT) tool
        - used by translators
    - Translation memories
        - "ICE" match: in-context match exact, 100% + context
        - Exact match: 100%
        - Fuzzy match: lower than 99%
    - Machine translation platforms
        - Rule-based machine translation (RBMT)
        - Statistical machine translation (SMT)
        - Post-editing: when translators or reviewers edit machine translations
        - Predictive machine translation
    - Google Translator Toolkit (GTT): Free CAT tool
        - Website: https://translate.google.com/toolkit
    - Subtitling platforms
        - .srt files
        - can add subtitles on YouTube in the "Creator Studio" in "Video Manager"
- Quality assurance tools
    - Formatting, grammar, punctuation, untranslated words, spacing
    - An automated report highlights issues

        