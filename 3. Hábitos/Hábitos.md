```dataviewjs
// Update this object
const trackerData = {
    entries: [],
    separateMonths: true,
    heatmapTitle: "Estudo",
}

// Path to the folder with notes
const PATH_TO_YOUR_FOLDER = "5. Diario";
// Name of the parameter you want to see on this heatmap
const PARAMETER_NAME = 'estudo';

// You need dataviewjs plugin to get information from your pages
for(let page of dv.pages(`"${PATH_TO_YOUR_FOLDER}"`).where((p) => p[PARAMETER_NAME])){
    trackerData.entries.push({
        date: page.file.name,
        // Use absolute file path so clicks open the exact note (for cases when you have multiple notes with the same name)
        filePath: page.file.path,
        intensity: page[PARAMETER_NAME],
    });
}

// Optional: set base path so new files are created here if missing
trackerData.basePath = PATH_TO_YOUR_FOLDER;

renderHeatmapTracker(this.container, trackerData);
```

--------
```dataviewjs
// Update this object
const trackerData = {
    entries: [],
    separateMonths: true,
    heatmapTitle: "Musculação",
}

// Path to the folder with notes
const PATH_TO_YOUR_FOLDER = "5. Diario";
// Name of the parameter you want to see on this heatmap
const PARAMETER_NAME = 'musculacao';

// You need dataviewjs plugin to get information from your pages
for(let page of dv.pages(`"${PATH_TO_YOUR_FOLDER}"`).where((p) => p[PARAMETER_NAME])){
    trackerData.entries.push({
        date: page.file.name,
        // Use absolute file path so clicks open the exact note (for cases when you have multiple notes with the same name)
        filePath: page.file.path,
        intensity: page[PARAMETER_NAME],
    });
}

// Optional: set base path so new files are created here if missing
trackerData.basePath = PATH_TO_YOUR_FOLDER;

renderHeatmapTracker(this.container, trackerData);
```

----
```dataviewjs
// Update this object
const trackerData = {
    entries: [],
    separateMonths: true,
    heatmapTitle: "Corrida/Cardio",
}

// Path to the folder with notes
const PATH_TO_YOUR_FOLDER = "5. Diario";
// Name of the parameter you want to see on this heatmap
const PARAMETER_NAME = 'corrida/cardio';

// You need dataviewjs plugin to get information from your pages
for(let page of dv.pages(`"${PATH_TO_YOUR_FOLDER}"`).where((p) => p[PARAMETER_NAME])){
    trackerData.entries.push({
        date: page.file.name,
        // Use absolute file path so clicks open the exact note (for cases when you have multiple notes with the same name)
        filePath: page.file.path,
        intensity: page[PARAMETER_NAME],
    });
}

// Optional: set base path so new files are created here if missing
trackerData.basePath = PATH_TO_YOUR_FOLDER;

renderHeatmapTracker(this.container, trackerData);
```

-----

