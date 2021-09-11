# Power BI

### Storage Mode

<table>
  <tr><th>Import</th><th>Direct Query</th></tr>
  <tr><td>Selected table and columns are imported in Power BI Desktop.</td><td>No data is imported in Power BI Desktop.</td></tr>
  <tr><td>Power BI Desktop uses the imported data to interact with the visualizations.</td><td>Power BI Desktop queries the live data source to interact with the visualizations. (Cloud Platform, Google Analytics, Database, etc.)</td></tr>
  <tr><td>Refreshing the data will reimport the entire dataset again.</td><td>Refreshing will be limited to the data source.</td></tr>
</table>

### Important Considerations 

`Direct Query` Mode is less suitable if :

- There is significant `load` time to get data from the back end source.
- A lot of users will use the reports.
- There are a lot of `RLS` row level security rules active on the dataset.

`Import` Mode

- `1GB` limit for datasets stored in shared capacities in a Power BI Service.
- Can only be refreshed `8` times a day by setting up a scheduled refresh.
