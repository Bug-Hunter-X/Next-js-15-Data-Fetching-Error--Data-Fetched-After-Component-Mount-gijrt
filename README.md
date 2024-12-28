# Next.js 15 Data Fetching Bug

This repository demonstrates a common data fetching issue in Next.js 15 where data is fetched within the component's body, causing the component to render with null data initially and an error. This issue arises because the data fetching occurs after the component has already mounted.

## Bug

The `pages/about.js` file contains the problematic code where data is fetched directly within the component. The `fetchData` function simulates fetching data from an external API.  The component renders before the data is available, which leads to errors.

## Solution

The `pages/about.js` (solution) file demonstrates how to resolve the issue using `async/await` and a loading state for proper data handling and UI responsiveness. 