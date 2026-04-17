# JavaScript Gantt Chart in Power BI

A Power BI custom visual integrating Syncfusion JavaScript Gantt chart into a Developer Visual using static sample task data.

## Project Overview

This repo builds a Power BI custom visual that renders a hierarchical Gantt chart inside the visual container. It uses `@syncfusion/ej2-gantt` for chart rendering and `powerbi-visuals-utils-formattingmodel` for formatting settings.

## Features

- Hierarchical tasks with subtasks
- Task field mapping for ID, name, start date, duration, progress, and dependencies
- Sample data in `src/datasource.ts`
- Formatting model in `src/settings.ts`

## Prerequisites

- Node.js and npm
- Power BI Visual Tools (`pbiviz`)
- Power BI report authoring environment

## Installation

1. Install dependencies:

   ```bash
   npm install
   ```

2. Start the developer server:

   ```bash
   npm start
   ```

## Usage

Open Power BI Desktop or Power BI service and load the developer visual from the Visualizations pane. The visual renders a Syncfusion Gantt chart inside a `div` with id `gantt`.

## Build and Package

- Run the Power BI CLI:

  ```bash
  npm run pbiviz
  ```

- Package the visual:

  ```bash
  npm run package
  ```

## Notes

The visual currently uses static sample data from `src/datasource.ts`. To connect real Power BI data, update the data source and task field mappings in `src/visual.ts`.
