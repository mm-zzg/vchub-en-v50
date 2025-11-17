# System.Tag.readHistory


## Description
Retrieve the historical records of the current tag, including the tag's path, value, quality code, time and aggregation mode.

## Grammar
```typescript
enum AggregationMode { "Raw", "Avg", "Max", "Min", "First", "Last", "Count", "Range", "CountOn", "CountOff", "DurationOn", "DurationOff" }

enum PeriodMode { "Second", "Minute", "Hour", "Day" }

interface ExtraOption { 
  timeout?: number; 
  noInterpolation?: boolean;
  ignoreBadQuality?: boolean; 
  includeBoundingValues?: boolean 
}

interface TagHistoryData {
  path: string;
  value: any;
  quality: string;
  time: string;
  aggregationMode: AggregationMode;
}

System.Tag.readHistory(
  start: Date | string,
  end: Date | string,
  tag: string | Array<string>,
  queryMode: "Raw",
  extraOption?: ExtraOption
): Promise<Array<TagHistoryData>>;

System.Tag.readHistory(
  start: Date | string,
  end: Date | string,
  tag: string | Array<string>,
  queryMode: "FixedPoints",
  aggregationMode: AggregationMode | Array<AggregationMode>,
  points: number,
  extraOption?: ExtraOption
): Promise<Array<TagHistoryData>>;

System.Tag.readHistory(
  startDate: string | Date,
  endDate: string | Date,
  tag: string | Array<string>,
  queryMode: "Periodic",
  aggregationMode: AggregationMode | Array<AggregationMode>,
  period: number,
  periodMode: PeriodMode,
  extraOption?: ExtraOption
): Promise<Array<TagHistoryData>>;

```
Parameter


## Code Example                                                                                                                                                                                                                                                                                                          
Retrieve the historical records of the raw values for the tag "Device:Temperature" between 2024-08-14 00:00:00 and 2024-08-15 00:00:00.
```typescript 
const value = await System.Tag.readHistory('2024-08-14 00:00:00', '2024-08-15 00:00:00', '@Device:Temperature','Raw'，{
  timeout: 30
});
console.log(value);


```
Retrieve the historical records of the variable "Device:Temperature" between 2024-08-14 00:00:00 and 2024-08-15 00:00:00 using the "FixedPoints" query mode, with "Avg" as the aggregation mode and a total of 30 data points.
```typescript 
const value = await System.Tag.readHistory('2024-08-14 00:00:00', '2024-08-15 00:00:00', '@Device:Temperature','FixedPoints','Avg',30, {
  timeout: 60,
  noInterpolation: true,
  ignoreBadQuality: true,
  includeBoundingValues: false
});
console.log(value);


```   
Retrieve the historical records of the variable "Device:Temperature" between 2024-08-14 00:00:00 and 2024-08-15 00:00:00, using the "Periodic" query mode, with "Max" as the aggregation mode, a period of 1, and "Minute" as the period mode.
```typescript 
const value = await System.Tag.readHistory('2024-08-14 00:00:00', '2024-08-15 00:00:00', '@Device:Temperature','Periodic','Max',1,'Minute', {
  timeout: 60,
  noInterpolation: true,
  ignoreBadQuality: true,
  includeBoundingValues: false
});
console.log(value);


```   



