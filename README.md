# WolfWorld 🐺

A sample multi-page static website about wolves, hosted on **Azure Static Web Apps**.

## Pages

| Page | File | Description |
|---|---|---|
| Home | `index.html` | Hero banner, quick stats, and highlight cards |
| Facts | `facts.html` | Biology, behaviour, and ecosystem facts |
| Species | `species.html` | Species overview, subspecies table, wolves vs. dogs |
| Gallery | `gallery.html` | Photo gallery with lightbox viewer |

## Structure

```
wolfapp/
├── index.html                 # Home page
├── facts.html                 # Wolf facts
├── species.html               # Species & subspecies
├── gallery.html               # Photo gallery
├── styles.css                 # Shared stylesheet
├── staticwebapp.config.json   # Azure Static Web Apps configuration
└── README.md
```

## Deploying to Azure Static Web Apps

1. Create a new **Azure Static Web App** in the [Azure Portal](https://portal.azure.com/).
2. Connect it to this GitHub repository.
3. Set the **app location** to `/` (repository root) and leave the API and output locations empty.
4. Azure will automatically provision a GitHub Actions workflow that builds and deploys the site on every push to `main`.

The `staticwebapp.config.json` file configures clean URL routes (e.g. `/facts` → `facts.html`), a 404 fallback, and security headers.