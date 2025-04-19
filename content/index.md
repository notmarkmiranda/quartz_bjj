---
title: Mark's Brazilian Jiu Jitsu Notes
draft: "false"
---
Inspired by [TCM BJJ](https://merryt.github.io/bjj-mindmap/) to take better BJJ notes.

Important dates:
- `20 SEP 2022` - First Fundamentals Class #whitebelt
- `25 JUN 2024` - Blue Belt Promotion #bluebelt 

Time since starting BJJ: 2 years, 7 months, 0 days
```dataviewjs
let start = new Date("2022-09-20");
let today = new Date();

let years = today.getFullYear() - start.getFullYear();
let months = today.getMonth() - start.getMonth();
let days = today.getDate() - start.getDate();

if (days < 0) {
  months -= 1;
  // rough fix for previous month’s days
  let prevMonth = new Date(today.getFullYear(), today.getMonth(), 0);
  days += prevMonth.getDate();
}

if (months < 0) {
  years -= 1;
  months += 12;
}

dv.paragraph(`Time since starting BJJ: ${years} years, ${months} months, ${days} days`);
```
