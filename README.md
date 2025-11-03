# GPS-Tracking-Repository

This repository preserves and shares GPS activity data for running and cycling in open formats. It is designed for INFO 4730 Module 10: Repository Project Part B.

## Rationale
The goal is to keep GPS activity data authentic, accessible, and reusable over time. GitHub is used because it provides version history, open access, and low-cost preservation with good documentation tools.

## User Group
- Athletes and fitness enthusiasts who want to review routes and progress
- Urban researchers studying mobility and exercise trends
- City planners who analyze routes for safety and infrastructure

## Information Needs and Gaps
Most fitness platforms keep data private or behind accounts. This repository fills the gap by publishing anonymized datasets with clear metadata in CSV and JSON. Users need:
- Open formats that load in common tools
- Basic metadata for time, distance, location, and elevation
- Integrity checks and a visible change history

## Organization
```
GPS-Tracking-Repository/
├── README.md
├── Running_Routes/          # 3 items
├── Cycling_Routes/          # 2 items
├── Metadata/                # templates and file-level metadata
└── Screenshots/             # workflow and structure images
```

## Ingestion
Files are uploaded with Git commits so author, timestamp, and changes are recorded. Each item includes a short metadata block in the file header or sidecar file.

## Metadata
A simplified ISO 19115 style is used. Key fields:
- activity_id
- activity_type (run or ride)
- date_time_utc
- distance_km
- duration_minutes
- avg_pace_or_speed
- elevation_gain_m
- start_lat, start_lon
- file_format (csv or json)
- citation

A CSV template is provided in `/Metadata/metadata_template.csv`.

## Collections and Items
- **Running_Routes**: three activities (`run1.csv`, `run2.csv`, `run3.json`)
- **Cycling_Routes**: two activities (`ride1.csv`, `ride2.json`)

## Access and Rights
The repository is public. Suggested license: **CC BY 4.0**. Cite as:
> Gaire, N. (2025). GPS Tracking Repository. GitHub. https://github.com/ng07900/GPS-Tracking-Repository

## Objectives
1. Preserve GPS data in open formats
2. Make datasets easy to reuse in coursework and research
3. Keep a clear history of updates

## Development, Testing, and Maintenance
- Build folders and README, upload five items, and add metadata
- Test by downloading and opening files in a notebook or spreadsheet
- Revisit each semester to validate links and formats

## Timetable
| Phase | Task | Time |
|---|---|---|
| Week 1 | Setup repository and folders | 1–2 days |
| Week 2 | Ingest five items with metadata | 2–3 days |
| Week 3 | Verify checksums and review | 1 day |
| Week 4 | Final review and share URL | 1 day |

## References
- Center for Research Libraries. (2006). *General factors to consider in evaluating digital repositories*.
- Digital Preservation Coalition. (n.d.). *Preservation action*.
- Purdue University Research Repository (PURR). (n.d.). *Preservation strategies*.
- DPWorkshop. (n.d.). *Preservation strategies*.
