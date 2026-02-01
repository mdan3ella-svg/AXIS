AXIS | Modern Design Standards & Codes

AXIS is a modern, single-file web application designed as an essential pocket tool for architects, designers, and students. It combines a searchable architectural encyclopedia with practical drafting utilities and robust accessibility features.

🚀 Features

1. The Design Library

A searchable, categorized database containing critical architectural data:

IBC Codes: Occupancy groups, egress width calculations, and fire resistance ratings.

Design Matrices: Adjacency matrices, bubble diagrams, and space standards.

Drafting Standards: Line weights, electrical symbols, and drawing conventions.

Accessibility: ADA ramp standards, toilet clearances, and more.

Dimensions: Standard door sizes, kitchen clearances, and furniture standards.

2. Utility Tools

Unit Converter: Real-time conversion between Feet, Inches, Millimeters, and Meters.

Scale Calculator: Instantly calculate real-world dimensions from scaled drawings (e.g., determine the actual length of a line drawn at 1/4" = 1'-0").

3. Accessibility Suite (A11y)

Designed to be inclusive for all users:

High Contrast Mode: Yellow-on-Black theme for low vision.

Dyslexia Support: Toggles a specialized font stack and increased letter spacing.

Text Sizing: Adjustable font sizes (Small, Default, Large).

Dark Mode: A slate-gray dark theme with teal accents.

4. Persistence

Bookmarks: Save frequently used articles for quick access.

Preferences: The app remembers your theme and font settings using localStorage.

🛠️ Installation & Usage

AXIS is built as a Single-File Application (SPA). It requires no server, build process, or installation wizard.

Download/Save:

Save the code as index.html on your computer.

Run:

Double-click index.html to open it in any modern web browser (Chrome, Firefox, Safari, Edge).

Offline Capability:

The application logic is self-contained.

Note: An internet connection is required upon the first load to fetch the styling (Tailwind CSS) and icons (Lucide) from the CDN. Once loaded, the browser typically caches these assets.

💻 Technical Details

Core: Vanilla JavaScript (ES6+). No frameworks required.

Styling: Tailwind CSS (via CDN) with CSS Variables for theming.

Icons: Lucide Icons (via CDN).

Fonts: Inter (UI) and JetBrains Mono (Data/Code).

Data Structure: All content is stored in a JSON-like database array within the <script> tag, making it easy to extend or modify.

🎨 Customization

To add new articles, open index.html in a text editor and locate the database array in the script section. Add a new object following this format:

{
    id: 101, // Unique ID
    title: "New Article Title",
    category: "Code", // Category ID matching the categories array
    tags: ["tag1", "tag2"],
    content: "HTML content goes here...",
    diagram: null // Or an SVG string
}


License

Open Source. Free to use and modify for educational and professional purposes.
