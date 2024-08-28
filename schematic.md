/fortune-teller-landing-page
│
├── /src
│   ├── /components
│   │   ├── FortuneTellerLogo.js
│   │   ├── FortuneTellerText.js
│   │   ├── FormStep1.js
│   │   ├── FormStep2.js
│   │   ├── PhoneNumber.js
│   │   └── ... (other reusable components)
│   │
│   ├── /config
│   │   ├── fortuneTellers.js
│   │   ├── emailMarketingTools.js
│   │   ├── partners.js
│   │   ├── textTemplates.js
│   │   ├── colorTemplates.js
│   │   ├── sources.js
│   │   ├── gtm.js
│   │   └── apiConfig.js
│   │
│   ├── /services
│   │   ├── activeCampaignService.js
│   │   ├── databaseService.js
│   │   ├── partnerService.js
│   │   ├── callCenterService.js
│   │   ├── gtmService.js
│   │   └── apiService.js
│   │
│   ├── /pages
│   │   ├── LandingPage.js
│   │   ├── FormPage1.js
│   │   ├── FormPage2.js
│   │   └── ... (other pages)
│   │
│   ├── /styles
│   │   ├── main.css
│   │   ├── colorTemplate1.css
│   │   ├── colorTemplate2.css
│   │   └── ... (other stylesheets)
│   │
│   ├── App.js
│   ├── index.js
│   └── ... (other entry points)
│
└── /public
    ├── /assets
    │   ├── /images
    │   │   ├── logo1.png
    │   │   ├── logo2.png
    │   │   └── ... (other images)
    │   │
    │   ├── /fonts
    │   │   └── ... (custom fonts)
    │   │
    │   ├── /scripts
    │   │   └── gtm.js
    │   │
    ├── index.html
    └── ... (other public files)



/src/components:

Purpose: This folder holds reusable components like the fortune teller's logo, text, form steps, and phone number input. By modularizing these elements, we can easily swap out or customize individual components for different fortune tellers without affecting the entire application.
Flexibility: Different fortune tellers can have their unique components if needed, while shared components remain reusable.
/src/config:

Purpose: This folder contains configuration files (fortuneTellers.js, emailMarketingTools.js, etc.) that define the specifics for different fortune tellers, email tools, partners, text templates, color templates, sources, and GTM settings.
Flexibility: By separating configurations from the logic, it allows the landing page to be easily reconfigured for different fortune tellers or campaigns by simply updating these files.
/src/services:

Purpose: Service files handle the logic for communicating with external systems like Active Campaign, the database, partners, call centers, and GTM. This keeps the application logic clean and centralized.
Flexibility: If a new service or API needs to be integrated, it can be done here without affecting other parts of the application.
/src/pages:

Purpose: This folder contains the different pages of the landing page, such as the main landing page and the form steps.
Flexibility: Each page is separate, making it easy to update or add new pages as needed.
/src/styles:

Purpose: Stylesheets are organized here, including a main stylesheet and separate files for different color templates.
Flexibility: Different fortune tellers or campaigns can have unique visual styles by simply swapping the corresponding CSS file.
/public/assets:

Purpose: This folder holds public assets like images, fonts, and GTM scripts.
Flexibility: It allows for easy updating of logos, images, and other static assets associated with each fortune teller.
App.js and index.js:

Purpose: These files are the main entry points for the React application, responsible for rendering the components and managing the app's state.
Flexibility: They connect everything together and can be configured to load the appropriate components and styles based on the current fortune teller or campaign.